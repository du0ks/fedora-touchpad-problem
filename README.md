# Huawei Matebook solution of touchpad issue on Fedora 
# If your touchpad is randomly being disabled when you boot the laptop try this solution!


 Put touchpad.sh file to /usr/bin than do chmod +x touchpad.sh on terminal

Now, we need to create service file for execute bash file when boot the pc.

Put touchpad.service file to /etc/systemd/system 

Now we need to enable and start the service so enter these commands to terminal:
sudo systemctl daemon-reload
sudo systemctl enable touchpad.service
sudo systemctl start touchpad.service

than reboot your pc, you can check logs with this command if you want to see service executed properly:
sudo systemctl status touchpad.service

good luck! 

***********************************************************************************************
