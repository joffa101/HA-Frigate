# HA-Frigate

## Setting up Frigate NVR on Home Assist
https://github.com/blakeblackshear/frigate/discussions/4041
file:///Users/glamb/Downloads/Installing.frigate.from.scratch.pdf


### Install ubuntu server

Tricks:
  Edit /etc/netplan/01-netcfg.yaml and add optional: true to any devices that may not always be available.
  sudo netplan apply

  apt-get install ntfs-3g 
  sudo mount -t ntfs-3g /dev/sdb2 /mnt/ntfs2/
