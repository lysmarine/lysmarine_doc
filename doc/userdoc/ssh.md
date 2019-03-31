
The  ssh server is disabled by default for security reason. Prior to enable it you should :

 - Change pi password with the `passwd` command.

 To start the service :
 ```
 sudo systemctl start ssh
 ```

 If you want ssh-server to start automatically at boot:
 ```
 sudo systemctl enable ssh
 ```

To disable the automatic launch at boot :

```
sudo systemctl stop ssh
```
