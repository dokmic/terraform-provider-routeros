# routeros_wifi_aaa (Resource)
*<span style="color:red">This resource requires a minimum version of RouterOS 7.13.</span>*

## Example Usage
```terraform
resource "routeros_wifi_aaa" "aaa1" {
  called_format   = "S"
  name            = "aaa1"
  password_format = ""
  username_format = "AA:AA:AA:AA:AA:AA"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) Name of the AAA profile.

### Optional

- `called_format` (String) Format of the `Called-Station-Id` RADIUS attribute.
- `calling_format` (String) Format of the `Calling-Station-Id` RADIUS attribute.
- `comment` (String)
- `disabled` (Boolean)
- `interim_update` (String) Interval at which to send interim updates about traffic accounting to the RADIUS server.
- `mac_caching` (String) Time to cache RADIUS server replies when MAC address authentication is enabled.
- `nas_identifier` (String) Value of the `NAS-Identifier` RADIUS attribute.
- `password_format` (String) Format of the `User-Password` RADIUS attribute.
- `username_format` (String) Format of the `User-Name` RADIUS attribute.

### Read-Only

- `id` (String) The ID of this resource.

## Import
Import is supported using the following syntax:
```shell
#The ID can be found via API or the terminal
#The command for the terminal is -> :put [/interface/wifi/aaa get [print show-ids]]
terraform import routeros_wifi_aaa.aaa1 '*1'
```