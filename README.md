# subsea-research
## Notes for Install of Subsea Traceroute collector

1. Install Rasperry OS on Raspberry Pi 3B+: https://www.raspberrypi.org/documentation/installation/installing-images/

2. Add an empty SSH file to root of Raspberry Pi OS MicroSD. This will enable SSH on the Pi.
https://www.raspberrypi.org/forums/viewtopic.php?t=210137

3. Create VPN on DigitalOcean Droplet to manage all Pis remotely.
- The DigitalOcean Droplet is Ubuntu 20.04n LTS
- OpenVPN-Install Script is the easist way to get VPN up and running:  https://github.com/angristan/openvpn-install
