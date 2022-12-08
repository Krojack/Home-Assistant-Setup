## My Hardware:
- [Intel NUC](https://www.amazon.com/gp/product/B018Q0GN60/) - i5-6260U
- [16GB RAM](https://www.amazon.com/gp/product/B07MBP5NBT/)
- 500GB SSD - A hand-me-down Samsung Drive from my primary computer

## Software setup:
- [Proxmox VE](https://proxmox.com/en/proxmox-ve) with 4 virtual servers running
  - 1st VM = Ubuntu server. This runs various things like:
    - MariaDB
    - InfluxDB
    - Pi-Hole
    - Other odds-n-ends services.
  - 2nd VM = HassOS. I followed [this guide](https://community.home-assistant.io/t/installing-home-assistant-using-proxmox/201835) to install everything from Proxmox to HA.
  - 3rd VM = Ubuntu Desktop. I can remote desktop into this and do various things. This is a 64G iSCSI mount from my NAS for it's storage.
  - 4th VM = Ubuntu Docker only. I run Portainer on it to manage the containers.

## Other hardware I have (all optional):
- 2 Synology NAS devices. 1 for file and backup storage, 1 for Plex media storage. Can also be used to create iSCSI storage for creating other VM servers.
- [GoControl HUSBZB-1](https://www.amazon.com/gp/product/B01GJ826F8/) - Zigbee & Z-wave USB dongle.
- [A USB extension cable](https://www.amazon.com/gp/product/B07VSG93G3/) - Needed to get the HUSBZB-1 away from your NUC.
- [Any USB HUB](https://www.amazon.com/gp/product/B08GYPDDLL/) - I plug my HUSBZB-1 and a Wyze sense hub. 2.0 hub is more than fast enough.
- [Bluetooth Dongle](https://www.amazon.com/gp/product/B07V1SZCY6/) - On-board bluetooth can be shielded from your system case. Get an external one to greatly extend it's range.

## Pics:
- [USB setup](https://i.imgur.com/9ctzb8b.jpg)
- [Hardware case](https://i.imgur.com/sEWwOGF.jpg) (out dated but still same rack)
  - Bottom: Intel NUC w/USB hub, 750GB Drive (now dead), 1 Synology NAS.
  - Top: Router, Cable modem.
- [HassOS VM Dashboard](https://i.imgur.com/gHKoafz.jpg) - HA runs fine with a 24GB drive partition and 2GB RAM.
