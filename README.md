# pilight
Some config stuff for [pilight](https://www.pilight.org) (and more) on [2016-09-23-raspbian-jessie-lite](https://www.raspberrypi.org/downloads/raspbian/)

raspi-config

# Usage
sudo service pilight stop
cd /etc
sudo rm -r pilight
sudo git clone https://github.com/JdenHartog/pilight.git

# Get info
nano /var/log/pilight.err
service pilight status

# Static IP (also done with Pi-hole)
sudo nano /etc/dhcpcd.conf
```
interface eth0<br>
static ip_address=192.168.1.100/24<br>
static routers=192.168.1.1<br>
static domain_name_servers=192.168.1.1
```

# Pi-hole
curl -L https://install.pi-hole.net | bash
