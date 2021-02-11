# My Hardware:
	- [Intel NUC](https://www.amazon.com/gp/product/B018Q0GN60/)
	- 16GB RAM
	- 256GB SSD

# Software setup:
	- Proxmox VE
	- 1st VM = Ubuntu server. This runs various things like MariaDB for HA history storage to my Plex server.
	- 2nd VM = HassOS. I followed this guide to install everything from Proxmox to HA.

# Other hardware I have (all optional):
	- Synology NAS. Used for Plex storage. Can also be used to create iSCSI storage for creating other VM servers.
	- GoControl HUSBZB-1 - Zigbee & Z-wave USB dongle.
	- A USB extension cable. - Needed to get the HUSBZB-1 away from your NUC.
	- Any USB HUB - I plug my HUSBZB-1 and a Wyze sense hub.

# Pics:
	- USB setup
	# Hardware case -
		- Bottom: Old Pi4, Intel NUC w/USB hub, 3TB Drive, Synology NAS w/USB hub.
		- Top: Router, Cable modem.

HassOS VM Dashboard - HA runs fine with a 24GB drive partition and 2GB RAM.
