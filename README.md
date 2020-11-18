# Snap to autostart bluetooth at boot

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

basically this app runs the **"hcicconfig hci0 up"** command


# Build

Follow the commands. you may need multipass support.


1 - git clone https://github.com/mauringo/autostart-bluetooth-snap.git


2 - cd autosrtart-bluetooth-snap


3 - snapcraft
