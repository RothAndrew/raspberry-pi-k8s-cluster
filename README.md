# raspberry-pi-k8s-cluster

Kubernetes Cluster on Raspberry Pi with K3s

## Instructions

> These instructions assume you have hardwired the Pi with ethernet. If you want to use Wi-Fi you definitely can, you'll just need to modify things a bit

1. Download [Raspbian Lite](https://www.raspberrypi.org/downloads/raspbian/)
1. Unzip the `.img` file
2. Download and install [Balena Etcher](https://www.balena.io/etcher/)
3. Flash the MicroSD card using Balena Etcher
4. Eject the card and put it back in
5. Add a file named `ssh` to the root directory of the card
6. put the card in the Raspberry Pi
7. SSH into the Pi by running `ssh pi@raspberrypi.local`
   1. The password is `raspberry`
   1. If you are on Windows and it can't find `raspberrypi.local` install [Bonjour](http://support.apple.com/kb/DL999)
8. 