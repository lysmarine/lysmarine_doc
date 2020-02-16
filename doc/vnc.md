# VNC 
Lysmarine provide the `x11vnc` server to allow desktop sharing of the `user` user.

The default VNC password is `changeme`. Plz set a new one with the command `vncpasswd`.


# Enabling / Disabling
 To start the service only for the current runtime:
 ```
 sudo systemctl start vnc.service
 ```

 If you want VNC to start automatically at boot:
 ```
 sudo systemctl enable vnc.service
 ```

To disable the automatic launch at boot :

```
sudo systemctl stop vnc.service
```

# Configuration
The default domain name of the chartplotter is `http://lysmarine.local`

Alternatively, You can find your local IP with the command `ip addr`

By default, vnc is listening on the port **5900**.