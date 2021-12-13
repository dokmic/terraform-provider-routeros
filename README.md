# Terraform Provider RouterOS

## Purpose

This provider is intended to be used with Router OS 7 and above. It makes use of the REST API introduced with Router OS v7.

### Todo for 0.1.0 (initial pre-release)

#### Resources:
- [x] Add resources for following objects normally found under `/ip` (Completed 2021-12-12)
    - [x] IP addresses (Completed 2021-12-10)
    - [x] DHCP client (Completed 2021-12-11)
    - [x] DHCP server (completed 2021-12-12)
    - [x] Pools (Completed 2021-12-12)
    - [x] Routes (Completed 2021-12-12)
- [x] Add resources for the following objects normally found under `/interface`
    - [x] VLANs (Completed 2021-12-11)
    - [ ] Bridge (_In Progress 2021-12-12_)
        - [x] Ports (Completed 2021-12-13)
        - [x] VLAN (Completed 2021-12-12)

#### Data:
- [ ] Add interface list as data object
- [ ] Add route list as data object
- [ ] Add IP address list as data object

## Usage

Please refer to the [documentation](docs/)

## Changelog

See [changelog.md](changelog.md)