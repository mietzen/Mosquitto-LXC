This is my personal documentation on how I installed Mosquitto in LXC.
```
apt install mosquitto mosquitto-clients
mosquitto_passwd -c /etc/mosquitto/passwd <USER>
```

```
nano /etc/mosquitto/conf.d/default.conf
```

```
allow_anonymous false
password_file /etc/mosquitto/passwd
```

```
systemctl restart mosquitto
```