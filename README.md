# pilight
Some config stuff for [pilight](https://www.pilight.org) (and more) on [2016-09-23-raspbian-jessie-lite](https://www.raspberrypi.org/downloads/raspbian/)

raspi-config

# Usage
sudo service pilight stop<br>
cd /etc/pilight<br>
sudo rm config.json<br>
sudo git clone https://github.com/JdenHartog/pilight.git<br>
sudo cp pilight/config.json config.json<br>
sudo rm -r pilight<br>

# Change title
sudo service pilight stop<br>
sudo nano /usr/local/share/pilight/index.html

# Get info
nano /var/log/pilight.err<br>
service pilight status<br>

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

optionally add Speedtest to Pihole WebUI<br>
https://blog.arevindh.com/2017/07/13/add-speedtest-to-pihole-webui/
