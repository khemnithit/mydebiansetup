# my debian setup

First,
`su`
and enter your root password.

## PC
```
apt update && apt upgrade && cd \
&& apt install task-thai-desktop flatpak gnome-software-plugin-flatpak syncthing obs-studio audacity gnome-boxes \
&& systemctl enable syncthing@khem.service \
&& systemctl start syncthing@khem.service \
&& flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo \
```
and reboot. Then,
`su`
and enter your root password.
```
cd \
&& flatpak install flathub org.shotcut.Shotcut \
&& flatpak install flathub com.spotify.Client \
```

## Server
```
apt update && apt upgrade && cd \
&& apt install curl \
&& cd \
&& curl -fsSL https://get.docker.com -o get-docker.sh \
&& sh get-docker.sh \
&& cd && cd /home/khem \
&& mkdir ./syncthing-app \
&& cd ./syncthing-app \
&& wget -O docker-compose.yml https://raw.githubusercontent.com/khemnithit/mydebiansetup/refs/heads/main/st_dc.yml \
&& cd && cd /home/khem \
&& mkdir ./filebrowser-app \
&& cd ./filebrowser-app \
&& wget -O docker-compose.yml https://raw.githubusercontent.com/khemnithit/mydebiansetup/refs/heads/main/fb_dc.yml \
&& cd \
&& curl -fsSL https://tailscale.com/install.sh | sh \
```
