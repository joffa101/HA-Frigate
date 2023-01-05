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

### Install Mint Cinamon 
37  sudo apt-get install openssh-server
   38  sudo systemctl is-enable ssh
   39  sudo systemctl is-enabled ssh
   40  sudo systemctl status ssh

50  sudo apt-get upgrade
   51  sudo apt install xrdp xorgxrdp
   52  sudo apt install -y freerdp2-x11
   53  echo env -u SESSION_MANAGER -u DBUS_SESSION_BUS_ADDRESS cinnamon-session>~/.xsession
   54  cat ~/.xsession
   55  sync
   56  xfreerdp /v:127.0.0.1
   57  sudo apt-get install wget gpg
   58  wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
   59  sudo install -D -o root -g root -m 644 packages.microsoft.gpg /etc/apt/keyrings/packages.microsoft.gpg
   60  sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list'
   61  ls
   62  rm -f packages.microsoft.gpg 
   63  sudo apt install apt-transport-https
   64  sudo apt-get update
   65  sudo apt-get upgrade
   66  sudo apt install code
   67  which code
   68  which vscode
   69  code
   70  apt-get install git
   71  sudo apt-get install git
   72  sudo add-apt-repository ppa:git-core/ppa 
   73  sudo apt-get update
   74  sudo apt-get install git
   75  which git



### Install Docker

https://docs.docker.com/engine/install/ubuntu/

  ### Install Portainer (to manage Docker)

  https://docs.portainer.io/start/install/server/docker/linux
  12 letter password "1 The flag ."

  ### Install Docker Compose
  
### Install HA via docker compose



  
