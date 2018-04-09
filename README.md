# Pi64-install
Pi64 install and configuration for deployment on a raspberry pi 3
The use of a Raspberry pi3 is required due to the need for a 64bit operating system for software compatibility.

# Instructions
download the pi64-lite.zip file from the following address: 
https://github.com/bamarni/pi64/releases

use etcher to write the image to at least a 4gb sd card, preferablly 8gb.

after boot look in your router for the raspberrypi ip address.
SSH into the pi with ssh pi@"your-ip"
you can use a program called putty to acomplish this.

then run the following commands
```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash 
sudo apt-get update
sudo apt-get install -y nano git curl make build-essential nodejs mongodb
sudo npm install -g node-gyp 
```