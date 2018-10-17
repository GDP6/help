# help
Help page for the project

## Useful Linux Commands 

### Server 
* `sudo lsof -i :X` lists processes running on port X. 
* `sudo kill -9 X` kills process with PID of X.
* `sudo python3 X.py &` runs X.py in the background. 
* `sudo ufw allow X/tcp` allow TCP connections to port X.

### Device 
* `sudo nano /etc/wpa_supplicant/wpa_supplicant.conf` opens file where WiFi can be configured. 

```
#Example of wpa_supplicant.conf file
country=GB
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
        ssid="WiFi-SSID"
        psk="WIFI-Password"
}
```
* `sudo wpa_cli -i wlan0 reconfigure` restarts wlan0.
* `ifconfig wlan0` to ensure wlan0 has an IP address.
* `curl http://www.google.com` again, to ensure there is internet access.
