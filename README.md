## My Hardware:
- [Intel NUC](https://www.amazon.com/gp/product/B018Q0GN60/)
- [16GB RAM](https://www.amazon.com/gp/product/B07MBP5NBT/)
- [256GB SSD](https://www.amazon.com/gp/product/B075RJS55D/)

## Software setup:
- [Proxmox VE](https://proxmox.com/en/proxmox-ve) with 3 virtual servers running
  - 1st VM = Ubuntu server. This runs various things like:
    - MariaDB
    - InfluxDB
    - Home Assistant
    - Plex Media Server
  - 2nd VM = HassOS. I followed [this guide](https://community.home-assistant.io/t/installing-home-assistant-using-proxmox/201835) to install everything from Proxmox to HA.
  - 3rd VM = Ubuntu Desktop. I can remote desktop into this and do various things. This is a 128G iSCSI mount from my NAS for it's storage.

## Other hardware I have (all optional):
- Synology NAS. Used for Plex storage. Can also be used to create iSCSI storage for creating other VM servers.
- [GoControl HUSBZB-1](https://www.amazon.com/gp/product/B01GJ826F8/) - Zigbee & Z-wave USB dongle.
- [A USB extension cable](https://www.amazon.com/gp/product/B07VSG93G3/) - Needed to get the HUSBZB-1 away from your NUC.
- [Any USB HUB](https://www.amazon.com/gp/product/B00L2442H0/) - I plug my HUSBZB-1 and a Wyze sense hub.

## Pics:
- [USB setup](https://i.imgur.com/9ctzb8b.jpg)
- [Hardware case](https://i.imgur.com/sEWwOGF.jpg)
  - Bottom: Old Pi4, Intel NUC w/USB hub, 3TB Drive, Synology NAS w/USB hub.
  - Top: Router, Cable modem.
- [HassOS VM Dashboard](https://i.imgur.com/2ohQ8Oa.jpg) - HA runs fine with a 24GB drive partition and 2GB RAM.
