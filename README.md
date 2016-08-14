# PiLight
Some config stuff for pilight

# Usage
sudo service pilight stop

sudo rm -r pilight

git clone https://github.com/JdenHartog/pilight.git



# Get info
nano /var/log/pilight.err

service pilight status

# Static IP /etc/dhcpcd.conf
interface eth0
static ip_address=192.168.0.10o/24
static routers=192.168.1.1
static domain_name_servers=192.168.1.1
