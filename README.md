# This repo is still WIP and not ready to be used!!!

# sap-netweaver-controlnetweaver-control [![Build Status](https://travis-ci.com/redhat-sap/sap-netweaver-control.svg?branch=master)](https://travis-ci.com/redhat-sap/sap-netweaver-control)

This role contains control operations for SAP Netweaver based applications (start, stop and restart)

## Requirements

This role is to be executed on a server where a SAP Netweaver based application is installed

## Role Variables

| variable | info | required? |
|:--------:|:----:|:---------:|
|sap_netweaver_control_instance_nr|Instance number of the system on which we want to operate|yes|
|sap_netweaver_control_function|Function that we want to execute|yes, `start,` `stop` or `restart`|

## Dependencies
This role has no dependencies

## Example Playbook

```yaml
    - hosts: servers
      roles:
      - role: sap-netweaver-control
```

## Example Inventory

```yaml
sap_netweaver_control_instance_nr: "00"
sap_netweaver_control_function: "start"
```

## License

GPLv3

## Author Information

Red Hat SAP Community of Practice
