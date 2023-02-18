# Fedora Touchpad Fix

## Purpose
In some laptops, touchpad is randomly disabling itself when you boot the computer.

### Files

* Download the files
* Put touchpad.sh file to ***/usr/bin*** 
* Execute the command in ***/usr/bin***
```
chmod +x touchpad.sh
```
### Creating the service

* Now, we need to create service file for execute bash file when boot the pc.
* Put touchpad.service file to ***/etc/systemd/system***
* Execute the commands 
```
sudo systemctl daemon-reload
sudo systemctl enable touchpad.service
sudo systemctl start touchpad.service
```

* TESTED ON FEDORA 32-33-34-35
