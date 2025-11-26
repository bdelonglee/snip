#### SYSTEM Echo my Public IP
curl http://ipecho.net/plain; echo


#### SYSTEM Linux Distro Infos
cat /etc/*-release


#### SYSTEM BASH CUT string length from left side
### echo "Hello World" | cut -c -4
## Hello World --> Hell
cut -c -4


#### SYSTEM BASH check if a file exists
if [[ -f /etc/resolv.conf ]]; then
    echo "/etc/resolv.conf exist"
fi
