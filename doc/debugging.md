#debugging audio 

first thing to try on raspberry: 
```
cd /opt/vc/src/hello_pi/
./rebuild.sh 
cd hello_audio
./hello_audio.bin 0 # For 3.5 audio jack
./hello_audio.bin 1 # For HDMI

```
next 

```
aplay --device plughw:CARD=Headphones /usr/share/sounds/alsa/Front_Center.wav

```

next 
```
aplay /usr/share/sounds/alsa/Front_Center.wav
```