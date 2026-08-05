## Void with... SwayFX


#XBPS packages install
```sh
sudo xbps-install void-repo-nonfree
```
```sh
sudo xbps-install -S firefox fastfetch yazi ghostty curl neovim swayfx seatd dbus
```

#SuperFile install
```sh
sudo bash -c "$(curl -sLo- https://superfile.dev/install.sh)"
```

#Services
```sh
sudo ln -s /etc/sv/dbus /var/service/
```
```sh
sudo ln -s /etc/sv/seatd /var/service/
```
#Configuration
```sh
sudo usermod -aG _seatd $(whoami)
```
Log out of current TTY session after the command above.
