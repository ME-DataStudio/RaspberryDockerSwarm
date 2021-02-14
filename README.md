# RaspberryDockerSwarm  
  
**based on:** https://devdojo.com/bobbyiliev/how-to-install-docker-and-docker-compose-on-raspberry-pi  
  
Create a docker swarm on four Raspberry Pi 4.  
  
Install RaspiOS and add a fie named ssh to the boot section of the SD-card.  

Change hostname: `sudo nano /etc/hostname` from 'raspberrypi' into e.g. 'pi1' or 'pinode1' or anyting else you fins usefull.
Do the same in `nano /etc/hosts`. Only change the name here not the local ip-address. Must be the same name as in `/etc/hostname`.
  
Put Sd-card in your raspberry and power on your Pi.  
