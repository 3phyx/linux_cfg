Odświeżanie repo
sudo zypper ref
Aktualizacja
sudo zypper update

Packman 6
tumbleweed:
sudo zypper ar -cfp 90 https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Tumbleweed/ packman

leap:
sudo zypper ar -cfp 90 'https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Leap_$releasever/' packman

vender -> packman
sudo zypper dup --from packman --allow-vendor-change

sudo zypper install opi
opi codecs

sudo zypper install flatpak
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

Snapy
Tumbleweed:
sudo zypper addrepo --refresh https://download.opensuse.org/repositories/system:/snappy/openSUSE_Tumbleweed snappy
Leap:
sudo zypper addrepo --refresh https://download.opensuse.org/repositories/system:/snappy/openSUSE_Leap_15.X snappy

sudo zypper --gpg-auto-import-keys refresh
sudo zypper dup --from snappy
sudo zypper install snapd
sudo systemctl enable --now snapd
sudo systemctl enable --now snapd.apparmor

Sterowniki:
https://www.opensuse-community.org/?ref=techhut.tv
