# my debian setup

**Not Tested !**

First,
`su`
and enter your root password.

## PC
```
apt update && apt upgrade \
&& apt install task-thai-desktop flatpak gnome-software-plugin-flatpak virt-manager obs-studio curl \
&& flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo \
&& cd \
&& curl -fsSL https://get.docker.com -o get-docker.sh \
&& sh get-docker.sh \
&& cd \
&& curl -fsSL https://tailscale.com/install.sh | sh \
```
and reboot. Then,
```
cd \
&& mkdir syncthing-app \
&& cd ./syncthing-app \
&& wget -O docker-compose.yml https
&& cd \
&& flatpak install flathub org.gnome.Epiphany \
&& flatpak install flathub org.shotcut.Shotcut \
&& flatpak install flathub com.spotify.Client \
```

## Server
```
apt update && apt upgrade \
&& apt install curl \
&& cd \
&& curl -fsSL https://get.docker.com -o get-docker.sh \
&& sh get-docker.sh \
&& cd \
&& curl -fsSL https://tailscale.com/install.sh | sh \
```
and reboot. Then,
```
cd \
&& mkdir syncthing-app \
&& cd ./syncthing-app \
&& wget -O docker-compose.yml https
```
