Aktualizacja kernela i pakietów <br />

sudo yum update kernel <br />
sudo yum update <br />
sudo yum upgrade <br />

Przeglądarka w konsoli <br />
sudo yum install links <br />
sudo yum install elinks <br />

Wget i 7zip <br />

sudo yum install wget <br />
sudo yum install p7zip <br />

Instalacja i konfiguracja Apache <br />

sudo yum install httpd <br />
firewall-cmd --add-service=http <br />
firewall-cmd --reload <br />
systemctl restart httpd.service <br />
systemctl start httpd.service <br />  
systemctl enable httpd.service <br />

Instalacja snapa <br />
sudo yum install snapd <br />
sudo systemctl enable --now snapd.socket <br />
sudo ln -s /var/lib/snapd/snap /snap <br />

Instalacja flatpaka <br />
sudo yum install flatpak <br />
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo <br />




