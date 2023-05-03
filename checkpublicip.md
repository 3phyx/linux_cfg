Windows Powershell (tested on windows 11) <br />

(Invoke-WebRequest ifconfig.me/ip).Content.Trim() <br />

Linux CLI <br />

dig +short myip.opendns.com @resolver1.opendns.com <br />
