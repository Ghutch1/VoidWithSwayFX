## Void with... SwayFX


#XBPS packages install
```sh
sudo xbps-install void-repo-nonfree
```
```sh
sudo xbps-install -S firefox fastfetch yazi ghostty curl neovim swayfx seatd dbus elogind mesa-dri
```
For Intel
```sh
sudo xbps-install -S mesa-vulkan-intel
```
For Radeon
```sh
sudo xbps-install -S mesa-vulkan-radeon
```
For Nvidia
```sh
sudo xbps-install -S nvidia nvidia-libs-32bit
```

#Services
```sh
sudo ln -s /etc/sv/dbus /var/service/
```
```sh
sudo ln -s /etc/sv/seatd /var/service/
```
```sh
sudo ln -s /etc/sv/elogind /var/service/
```
#Configuration
```sh
sudo usermod -aG _seatd $(whoami)
```
Log out of current TTY session after the command above.
