# raspberry-pi-k8s-cluster

Kubernetes Cluster on Raspberry Pi with K3s

## Instructions

> These instructions assume you have hardwired the Pi with ethernet. If you want to use Wi-Fi you definitely can, you'll just need to modify things a bit

### Hardware Setup and Login

1. Download [Raspbian Lite](https://www.raspberrypi.org/downloads/raspbian/)
2. Unzip the `.img` file
3. Download and install [Balena Etcher](https://www.balena.io/etcher/)
4. Flash the MicroSD card using Balena Etcher
5. Eject the card and put it back in
6. Add a file named `ssh` to the root directory of the card
7. put the card in the Raspberry Pi
8. SSH into the Pi by running `ssh pi@raspberrypi.local`
   1. The password is `raspberry`
   2. If you are on Windows and it can't find `raspberrypi.local` install [Bonjour](http://support.apple.com/kb/DL999)

### Configuration

1. Change the password
   1. Run `sudo raspi-config`
   2. Pick "Change User Password"
   3. Follow the instructions to change the password
1. Change the hostname
   1. Run `sudo raspi-config`
   2. Pick "Network Options"
   3. Pick "Hostname"
   4. Follow the instructions to change the hostname
   5. Reboot by running `sudo reboot now`
2. Expand the filesystem
   1. Run `sudo raspi-config`
   2. Pick "Advanced Options"
   3. Pick "Expand Filesystem"