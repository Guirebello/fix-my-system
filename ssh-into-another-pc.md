Fisrt you gotta have openssh client and server on the respective machines

## Enable sshd
```shell
sudo systemctl enable --now sshd
```
```shell
sudo systemctl status sshd
```

## Grab the ip
Them, in the machine you want to connect, type:

```sh
ip addr
```
Now grab the inet ip from your internet station (wlan0 for example)

## SSH into the machine
now that you have the ip and the username of wich you want to connect, you just gotta ssh into the ip

```sh
ssh username@ipadress
```