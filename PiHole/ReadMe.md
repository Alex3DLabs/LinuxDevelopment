# PiHole

https://pi-hole.net

https://github.com/pi-hole/pi-hole/#one-step-automated-install


Setting a static IP Address

  ```
sudo nmcli c mod "Wired connection 1" ipv4.addresses 192.168.1.5/24 ipv4.method manual

sudo nmcli con mod "Wired connection 1" ipv4.gateway 192.168.1.1

sudo nmcli con mod "Wired connection 1" ipv4.dns 192.168.1.1

OR

sudo nmcli con mod "Wired connection 1" ipv4.dns "8.8.8.8,1.0.0.1"

sudo nmcli c down "Wired connection 1" && sudo nmcli c up "Wired connection 1"
```





Old Notes
sudo nmcli con mod "Wired connection 1" \
  ipv4.addresses "192.168.1.5/24" \
  ipv4.gateway "192.168.1.1" \
  ipv4.dns "192.168.1.1,1.1.1.1" \
  ipv4.dns-search "foradori.local" \
  ipv4.method "manual"
