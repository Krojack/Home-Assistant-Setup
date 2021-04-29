## My Hardware:
- [Intel NUC](https://www.amazon.com/gp/product/B018Q0GN60/)
- [16GB RAM](https://www.amazon.com/gp/product/B07MBP5NBT/)
- [256GB SSD](https://www.amazon.com/gp/product/B075RJS55D/)

## Software setup:
- [Proxmox VE](https://proxmox.com/en/proxmox-ve) with 3 virtual servers running
  - 1st VM = Ubuntu server. This runs various things like:
    - MariaDB
    - InfluxDB
    - Other odds-n-ends like MQTT broker and someday ZwaveJS2MQTT
  - 2nd VM = HassOS. I followed [this guide](https://community.home-assistant.io/t/installing-home-assistant-using-proxmox/201835) to install everything from Proxmox to HA.
  - 3rd VM = Ubuntu Desktop. I can remote desktop into this and do various things. This is a 64G iSCSI mount from my NAS for it's storage.

## Other hardware I have (all optional):
- Synology NAS. Used for Plex storage. Can also be used to create iSCSI storage for creating other VM servers.
- [GoControl HUSBZB-1](https://www.amazon.com/gp/product/B01GJ826F8/) - Zigbee & Z-wave USB dongle.
- [A USB extension cable](https://www.amazon.com/gp/product/B07VSG93G3/) - Needed to get the HUSBZB-1 away from your NUC.
- [Any USB HUB](https://www.amazon.com/gp/product/B08GYPDDLL/) - I plug my HUSBZB-1 and a Wyze sense hub. 2.0 hub is more than fast enough.
- [Bluetooth Dongle](https://www.amazon.com/gp/product/B07V1SZCY6/) - On-board bluetooth can be shielded from your system case. Get an external one to greatly extend it's range.

## Pics:
- [USB setup](https://i.imgur.com/9ctzb8b.jpg)
- [Hardware case](https://i.imgur.com/sEWwOGF.jpg)
  - Bottom: Intel NUC w/USB hub, 750GB Drive (now dead), Synology NAS w/USB hub.
  - Top: Router, Cable modem.
  - (Not in photo) 2 2TB USB drives plugged into the NUC. NAS is getting full so I move low watched Plex videos over to these. I rsync one drive to the other as a backup.
- [HassOS VM Dashboard](https://i.imgur.com/gHKoafz.jpg) - HA runs fine with a 24GB drive partition and 2GB RAM.
