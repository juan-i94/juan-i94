# Dev Log

## 2024-08-20
Installed Ubuntu Server on my old computer, took me a good 3 or 4 hours and couldn't get the VPN (WireGuard) to work

What I learnt:
SSH, Static IP's, SUDO, updating the system, unattended-upgrades, update-notifier, NANO, network configuration, Samba, Cockpit

## 2024-10-22

Installed Jellyfin on the server.
Finally Fixed the WireGuard VPN. The problem was that my ISP didn't give me access to the router configuration. 
I found the router password online and I was able to forward the necessary ports to make it work. The VPN works via DuckDNS

Learnt:
Users, Groups, Permissions, VPN's, DNS, Port Forwarding, 

## 2024-11-16

Installed Syncthing as alternative to Samba, still not sure which one I prefer. 
One is a manual way of sharing files and the other one syncs automaticlly but I'm looking for an alternative to Google Photos, and Syncthing doesn't really work for my laptop as it has low storage capacity and my need is just to upload things to the server not have the files on both devices.

## 2024-11-19

- Learning to use github while writing an html doc (free code camp)

## 2024-11-26

Installed SteamCMD
Installed a Valheim Server.
Installed UFW
Installed Termius on desktop and laptop (I had been using it on my phone previously)

Bought an Arduino UNO, still not sure what to do with it. It came with a few sensors, cables, leds, switches. Maybe I'll try setting up an irrigation system for my gf.

Learnt: 
Curl, reading systemd logs, setting up a service.
When I installed UFW it messed up a lot of my stuff as I didn't make exceptions for the VPN port for example. so I had to do that. Also learnt a bit more about port forwarding as I had a little trouble with the Valheim Server ports.
A little C++

## 2024-11-29

Tried Installing mods to the Valheim Server, something didn't work. had to reinstall everything. In the end it worked.

I learnt:
BACK UPS ARE SUPER SO VERY IMPORTANT
I started using Termius' SFTP option to move around the server files, like the world save files.
Had a little intro to SSH keys but didn't set it up yet

## 2024-12-03

Tried a bit more arduino, mostly hardware side.

## 2024-12-04

Found an old HDD and trying to hook it up to the server
running lsblk shows the list of "block devices"
sudo fdisk -l gives me a more detailed disk partition table.

sudo mount /dev/sdb1 /mnt/tempdisk This mounts the HDD to a temp dir
sudo umount /mnt/tempdisk

formatted with mkfs.ext4 and permanently mounted it to /mnt/sdb1