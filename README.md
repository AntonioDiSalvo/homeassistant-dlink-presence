## A D-Link AP/router device tracker for Home Assistant

Will return a list of MAC addresses that are connected to the wireless interface of the D-Link device.  
Useful for tracking who is at home and who is away.

Queries the device over telnet. Make sure to enable telnet for this to work.

### Configuration example

```
device_tracker:
  - platform: dva_presence
    host: 192.168.1.2 # ap
    username: admin
    password: !secret ap_password
```

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)
