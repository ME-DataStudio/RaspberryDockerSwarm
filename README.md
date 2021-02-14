# Raspberry Docker Swarm  
  
**based on:** https://medium.com/@henrique.menezes/building-a-raspberry-pi-cluster-with-docker-swarm-b457fb2f61a1  
  
Create a docker swarm on four Raspberry Pi 4.  
  
Install RaspiOS and add a file named ssh to the boot section of the SD-card. Put Sd-card in your raspberry pi and turn it on.  
Find the ip-address of your Pi in the list of connetced devices in your router/access point. SSH into your Pi from an other computer.  
`ssh pi@192.168.1.21` for example. Default username is `pi`, default password `raspberry`.  
Run `sudo raspi-config` and change password via `1 System settings - S3 password` and then change hostename `S4 hostname` into e.g. `pi1`.    

### _Note: you can change hostname also like this:_  
`sudo nano /etc/hostname` from 'raspberrypi' into e.g. 'pi1'. Do the same in `nano /etc/hosts`. Only change the name here not the local ip-address. Must be the same name as in `/etc/hostname`.
  
  
### To Do  
- boot to USB
- static ip-address
- install Docker `curl -fsSL https://get.docker.com | sh`
- setup docker swarm `sudo docker swarm init --advertise-addr 192.168.0.20`
- setup datastax
