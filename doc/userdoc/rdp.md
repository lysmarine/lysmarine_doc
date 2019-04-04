Lysmarine provide xrdp to allow a remote RDP connections.


 To start for the service only for the current runtime:
 ```
 sudo systemctl start xrdp.service
 ```

 If you want xrdp to start automatically at boot:
 ```
 sudo systemctl enable xrdp.service
 ```

To disable the automatic launch at boot :

```
sudo systemctl stop xrdp.service
```
