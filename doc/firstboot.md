
# Set local time
By default, lysmarine time is set on GMT.
To choose your location, navigate to `/usr/share/zoneinfo/`
Find the file corresponding to your location (`America/Montreal` in this example)
Then copy it into `/etc/localtime`  folder.
```
sudo cp /usr/share/zoneinfo/America/Montreal /etc/localtime
```

# Passwords
Default passwords are:
> User:`user`<br> 
> Password:`changeme` 

> User:`root`<br> 
> Password:`changeme` 

As their name says, you are strongly advised to change them, 
 - Change user password with the command :  `passwd`
 - Change root password with the command :  `sudo passwd root`
 - Change VNC password with the command  :  `vncpasswd`

Signalk don't have any accound made by default, so plz create one before someone malicious do it :
`Go to Menu` > `System` > `SignalK`  Press Login button upper right and choose your username & password. 


### Aditional configurations
> __TODO:__ systemd services

