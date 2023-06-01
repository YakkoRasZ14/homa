### Update & upgrade first your VPS for Debian 10 & 11

  ```html
  apt update -y && apt upgrade -y && apt dist-upgrade -y && reboot 

  ```

### Update & upgrade First your VPS for Ubuntu 18.04 & 20.04

  ```html
  apt-get update && apt-get upgrade -y && apt dist-upgrade -y && update-grub && sleep 2 && reboot

   ```
### Root Access.Password = #123VPSKu

```html
sudo wget -O ./default.sh 'https://script.gegevps.com/default.sh' && sudo chmod +x ./default.sh && sudo ./default.sh && sudo rm -rf ./default.sh
  
   ```
### Installation scripts

  ```html
  sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt update && apt install -y bzip2 gzip coreutils screen curl && wget https://raw.githubusercontent.com/YakkoRasZ14/homa/main/setup.sh && chmod +x setup.sh && sed -i -e 's/\r$//' setup.sh && screen -S setup ./setup.sh

  ```
 
 ### Copy & paste to your VPS if <img src="https://img.shields.io/badge/Error-red.svg">(WG Only)
 ### Wireguard

  ```html
  echo "deb http://deb.debian.org/debian/ unstable main" >/etc/apt/sources.list.d/unstable.list
printf 'Package: *\nPin: release a=unstable\nPin-Priority: 90\n' >/etc/apt/preferences.d/limit-unstable
apt update
apt install -y wireguard-tools iptables iptables-persistent
apt install -y linux-headers-$(uname -r)
 
  ```
 
   ```html
systemctl restart wg-quick@wg0

  ```

## Description :
Experimental Script
# homa
