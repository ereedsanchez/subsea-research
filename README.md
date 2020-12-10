# subsea-research
## Notes for Install of Subsea Traceroute collector

1. Install Rasperry OS on Raspberry Pi 3B+: https://www.raspberrypi.org/documentation/installation/installing-images/

2. Add an empty SSH file to root of Raspberry Pi OS MicroSD. This will enable SSH on the Pi.
https://www.raspberrypi.org/forums/viewtopic.php?t=210137

3. Create VPN on DigitalOcean Droplet to manage all Pis remotely.
- The DigitalOcean Droplet is Ubuntu 20.04n LTS
- OpenVPN-Install Script is the easist way to get VPN up and running:  https://github.com/angristan/openvpn-install

4. Create users with ./openvpn-install.sh, Example user: CornIsland will create CornIsland.ovpn file. 
5. SCP file to the Pi. 

On CLient Pi (or Linux system)

1. scp root@198.199.71.241:/home/vpn/CornIslandCLTI.ovpn /home/Downloads/
2. mv /home/Downloads/CornIslandCLTI.ovpn /etc/openvpn/
3. sudo openvpn --config CornIslandCLTI.ovpn
4. Set up Autostart openvpn https://support.vpnsecure.me/articles/getting-started/linux-autostart-openvpn-in-systemd-ubuntu
5. Autostart ssh : https://securityjedi.com/?p=210
