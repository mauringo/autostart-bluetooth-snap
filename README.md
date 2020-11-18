summary: app to autostart bluetooth at boot.

using Ubuntu Core devices it is not always possible to access via SSH and bluez 
usually doesn't start up the bluetooth at boot. Sometimes is note event possible 
to access the device via SSH. 

usage: 
1 - install bluez to allow bluetooth usage:
"sudo snap install bluez"
2 - check dongle compatibility
"sudo bluez.hciconfig"
3 - install bluetooth autosatart 
"sudo snap install bluetooth-autostart"

basically this app runs the "hcicconfig hci0 up" command
