# If your touchpad is randomly disabling when you boot the system try this solution!


Put touchpad.sh file to ***/usr/bin*** and ***chmod +x touchpad.sh*** (go to /usr/bin in terminal too)

Now, we need to create service file for execute bash file when boot the pc.

Put touchpad.service file to ***/etc/systemd/system***


**sudo systemctl daemon-reload**

**sudo systemctl enable touchpad.service**

**sudo systemctl start touchpad.service**

TESTED ON FEDORA 32-33-34-35
***********************************************************************************************
