if you cannot run docker-compose:

## 1. See if the application is up
```sh
systemctl status docker
```
if its not active, start it
## 2. Start docker
```sh
sudo systemctl start docker
```
now just run docker compose