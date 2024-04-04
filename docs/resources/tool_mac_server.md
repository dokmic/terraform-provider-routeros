# routeros_tool_mac_server (Resource)


## Example Usage
```terraform
resource "routeros_tool_mac_server" "test" {
  allowed_interface_list = "LAN"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `allowed_interface_list` (String) List of interfaces for MAC Telnet access.

### Optional


### Read-Only

- `id` (String) The ID of this resource.

## Import
Import is supported using the following syntax:
```shell
terraform import routeros_tool_mac_server.test .
```