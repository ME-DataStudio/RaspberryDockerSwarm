# RaspberryDockerSwarm  
  
**based on:** https://devdojo.com/bobbyiliev/how-to-install-docker-and-docker-compose-on-raspberry-pi  
  
Create a docker swarm on four Raspberry Pi 4.  
  
Install RaspiOS and add a file named ssh to the boot section of the SD-card. Put Sd-card in your raspberry pi and turn it on.  
Find the ip-address of your Pi in the list of connetced devices in your router/access point. SSH into your Pi from an other computer.  
`ssh pi@192.168.1.21` for example. Default username is `pi`, default password `raspberry`.  
Run `sudo raspi-config` and change password via `1 System settings - S3 password` and then change hostename `S4 hostname` into e.g. `pi1`.    

##_Note:_
     you can change hostname also like this:  
     `sudo nano /etc/hostname` from 'raspberrypi' into e.g. 'pi1' or 'pinode1' or anyting else you fins usefull.
      Do the same in `nano /etc/hosts`. Only change the name here not the local ip-address. Must be the same name as in `/etc/hostname`.
  
Put Sd-card in your raspberry and power on your Pi.  
  
### To Do  
- boot to USB
- static ip-address
- install Docker
- setup docker swarm
- setup datastax
