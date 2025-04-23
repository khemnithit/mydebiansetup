# my debian setup

**Not Tested !**

First,
`su`
and enter your root password.

## PC
```
apt update && apt upgrade \
&& apt install task-thai-desktop flatpak gnome-software-plugin-flatpak virt-manager obs-studio \
&& flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo \
&& cd \
&& curl -fsSL https://get.docker.com -o get-docker.sh \
&& sh get-docker.sh \

```
and reboot. Then,
```
cd \
&& mkdir syncthing-app \
&& cd ./syncthing-app \
&& wget -O docker-compose.yml https
```
