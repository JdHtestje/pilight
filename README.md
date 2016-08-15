# PiLight
Some config stuff for pilight on RASPBIAN JESSIE LITE

# Usage
sudo service pilight stop

sudo rm -r pilight

git clone https://github.com/JdenHartog/pilight.git



# Get info
nano /var/log/pilight.err

service pilight status

# Static IP /etc/dhcpcd.conf
interface eth0<br>
static ip_address=192.168.1.100/24<br>
static routers=192.168.1.1<br>
static domain_name_servers=192.168.1.1
