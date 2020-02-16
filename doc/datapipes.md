# GPS

```
USBgps ==> gpsd ==> signalk => freeboard-sk 
            ||         ||
            ||         |==> signalk-to-nmea0183 ==> OpenCPN
            ||     
            |==> pypilot
```

`signalk-to-nmea0183` is a signalk plugin pre-configured to emit `nmea0183` string over tcp on the port `10110`.
Opencpn is configured to listen on this port for `nmea0183` sentences.  

More precision on how the physical GPS dongle, gpsd and signalk interact is available un the [GPS](doc/gps.md) section.




# Time

```
          Internet ==> chrony ==> Linux time 
                         ||
          RTC(if any) ===>|

              [OR]

USBgps ==> gpsd ==> signalk => signalk-time-plugin ==> linux time (date)

```
At boot and every 30min `signalk-time-plugin` check if `chrony` have been able do sync with the internet time. 
If not, `signalk-time-plugin` will take the GPS time and set the linux time throu the command `date`.




# Charts 

```
/home/user/harts ==>|
                   ||
              /srv/charts ==> signalK charts plugin ==> freeboard-sk
                   || 
                   |==> Opencpn
```

# Pypilot

```
GPS ==> gpsd ==>|
               ||
boat_imu ==> pypilot ==> autopilot
               || 
               |==> pypilot_web(server) ==> pypilot_webapp(nativfier)
               ||
               |==> pypilot_control
               ||
               |==> pypilot_calibration 
```
