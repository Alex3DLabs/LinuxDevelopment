# PiHole

https://pi-hole.net

https://github.com/pi-hole/pi-hole/#one-step-automated-install



sudo nmcli con mod "Wired connection 1" \
  ipv4.addresses "192.168.1.5/24" \
  ipv4.gateway "192.168.1.1" \
  ipv4.dns "192.168.1.1,1.1.1.1" \
  ipv4.dns-search "foradori.local" \
  ipv4.method "manual"
