# my debian setup

**Not Tested !**

First,
`su`
and enter your root password.

## PC
*check package list before start*
```
echo I am about to start \
&& apt update && apt upgrade && cd \
&& apt install task-thai-desktop flatpak gnome-software-plugin-flatpak virt-manager obs-studio curl syncthing audacity \
&& systemctl enable syncthing@khem.service \
&& systemctl start syncthing@khem.service \
&& flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo \
&& cd \
&& curl -fsSL https://tailscale.com/install.sh | sh \
&& echo we are done when i say we are done \
```
and reboot. Then,
```
echo let me cook \
&& cd \
&& flatpak install flathub org.gnome.Epiphany \
&& flatpak install flathub org.shotcut.Shotcut \
&& flatpak install flathub com.spotify.Client \
&& echo we are done \
```

## Server
```
apt update && apt upgrade && cd \
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
