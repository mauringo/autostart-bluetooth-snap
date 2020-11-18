# Snapp to autostart bluetooth at boot

## Why?
Using Ubuntu Core devices it is not always possible to access via SSH. furthermore, bluez usually doesn't start up the bluetooth at boot. In the worst cases is not even possible to access the device via SSH.

## Usage
 1 - install bluez to allow bluetooth:
        "sudo snap install bluez" 
2 - check dongle compatibility:
     "sudo bluez.hciconfig"   --> the log must show up the HCI devices with their state
3 - install bluetooth autosatart:
 "sudo snap install bluetooth-autostart"
 
**Enjoy**

basically this app runs the "hcicconfig hci0 up" command
# Files

StackEdit stores your files in your browser, which means all your files are automatically saved locally and are accessible **offline!**
