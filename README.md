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
  
  **Stop cloud-init**. Create an empty file to prevent the service from starting
  sudo touch /etc/cloud/cloud-init.disabled
  
### Install Docker

https://docs.docker.com/engine/install/ubuntu/

  ### Install Portainer (to manage Docker)

  https://docs.portainer.io/start/install/server/docker/linux
  12 letter password "1 The flag ."

  ### Install Docker Compose
  
### Install HA via docker compose



  
