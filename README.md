# ThingSpeak for Raspberry Pi
Forked from sirleech's thingspeak <https://github.com/sirleech/thingspeak>

ThingSpeak Python scripts for the Raspberry Pi.

Example: https://thingspeak.com/channels/14416

## Installation Instructions
```
$ sudo apt-get install python-psutil
$ cd /opt
$ sudo git clone https://github.com/nicholaswilde/thingspeak-raspberry-pi.git
$ cd thingspeak-raspberry-pi
$ sudo chmod +x thingspeak_cpu_loop.py
$ python thingspeak_cpu_loop.py
$ sudo nano /etc/rc.local
```
Add the following line right above the ```exit 0``` command in your ```/etc/rc.local``` file.

```
...
python /etc/thingspeak-raspberry-pi/thingspeak_cpu_loop.py

exit 0
```

Reboot your Raspberry Pi

```$ sudo reboot```



