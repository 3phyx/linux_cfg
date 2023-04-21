Odświeżanie repo:<br />
sudo zypper ref<br />
Aktualizacja:<br />
sudo zypper update<br />

Packman 6<br />
tumbleweed:<br />
sudo zypper ar -cfp 90 https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Tumbleweed/ packman<br />

leap:<br />
sudo zypper ar -cfp 90 'https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Leap_$releasever/' packman<br />

vender -> packman:<br />
sudo zypper dup --from packman --allow-vendor-change<br />

Codecs:<br />
sudo zypper install opi<br />
opi codecs<br />

Flatpak:<br />
sudo zypper install flatpak<br />
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo<br />

Snapy:<br />
Tumbleweed:<br />
sudo zypper addrepo --refresh https://download.opensuse.org/repositories/system:/snappy/openSUSE_Tumbleweed snappy<br />
Leap:<br />
sudo zypper addrepo --refresh https://download.opensuse.org/repositories/system:/snappy/openSUSE_Leap_15.X snappy<br />

sudo zypper --gpg-auto-import-keys refresh<br />
sudo zypper dup --from snappy<br />
sudo zypper install snapd<br />
sudo systemctl enable --now snapd<br />
sudo systemctl enable --now snapd.apparmor<br />

Sterowniki:<br />
https://www.opensuse-community.org/?ref=techhut.tv<br />
