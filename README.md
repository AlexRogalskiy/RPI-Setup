# Setup Raspberry Pi (headless) 🔧
How to prepare and setup a Raspberry Pi. 

1. Download the latest version of [Raspbian](https://www.raspberrypi.org/downloads/raspbian/) and flash your micro SD card with [Etcher](https://etcher.io/)

2. Copy the **ssh** and **wpa_supplicant.conf** files from the **setup folder** to the SD card (boot) 

3. Edit the **wpa_supplicant.conf** in a text editor to match your wifi settings. Insert the card to the raspberry pi

4. In terminal ssh into the pi: ```sudo ssh pi@raspberrypi.local```<br>*Defult password is 'raspberry'. To change password use the 'passwd' command*

5. Update the pi: ```sudo apt-get update && sudo apt-get upgrade```<br>

6. Install **nodejs** : ```sudo apt-get install nodejs npm git-core```<br>

7. Reboot ```sudo reboot```

*Optional:* install nettalk for easy file sharing ```sudo apt-get install netatalk```<br>

# Setup OrangePi  🔧
How to prepare and setup a Orange Pi. 

1. Download the hardwhere specific version of [Raspbian](http://www.orangepi.org/downloadresources/) and flash your micro SD card with [Etcher](https://etcher.io/)

2. Connect the Orange Pi via USB to your computer.
3. In terminal search for the usb port ```ls /dev/tty.*```
4. Log on to the Orange pi ```screen [USB-PORT-NAME] 115200```
5. Login with user: **root** and pasword: **1234**<br>*The Orange pi wil ask you to change your pasword*
6. Setup the wifi ```nmtui-connect```

5. Update with: ```sudo apt-get update && sudo apt-get upgrade```<br>

6. Reboot ```sudo reboot```

*Optional:* install nettalk for easy file sharing ```sudo apt-get install netatalk```<br>
