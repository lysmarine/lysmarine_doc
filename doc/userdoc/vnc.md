Lysmarine provide the x11vnc server to allow desktop sharing of the pi user.

The service is disabled by default for security reason. Prior to enable it you should :

 - set a VNC password with the command `vncpasswd`.

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

By default, vnc is listening on the port **5900**. You can find your local IP with the command `ip addr`
