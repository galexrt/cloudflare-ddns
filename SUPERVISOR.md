## Hassio Supervisor Network Info JSON Response

`http://supervisor/network/info`

```json
{
  "result": "ok",
  "data": {
    "interfaces": [
      {
        "interface": "eth0",
        "type": "ethernet",
        "enabled": true,
        "connected": true,
        "primary": true,
        "ipv4": {
          "method": "auto",
          "address": [
            "IP_ADDRESS"
          ],
          "nameservers": [
            "DNS_SERVER"
          ],
          "gateway": "LOCAL_GATEWAY"
        },
        "ipv6": {
          "method": "auto",
          "address": [
            "NON_LINK_LOCAL",
            "LINK_LOCAL"
          ],
          "nameservers": [],
          "gateway": "LOCAL_GATEWAY"
        },
        "wifi": null,
        "vlan": null
      },
      {
        "interface": "wlan0",
        "type": "wireless",
        "enabled": false,
        "connected": false,
        "primary": false,
        "ipv4": {
          "method": "disabled",
          "address": [],
          "nameservers": [],
          "gateway": null
        },
        "ipv6": {
          "method": "disabled",
          "address": [],
          "nameservers": [],
          "gateway": null
        },
        "wifi": null,
        "vlan": null
      }
    ],
    "docker": {
      "interface": "hassio",
      "address": "172.30.32.0/23",
      "gateway": "172.30.32.1",
      "dns": "172.30.32.3"
    },
    "host_internet": true,
    "supervisor_internet": true
  }
}
```
