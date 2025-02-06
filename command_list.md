# REPAIR SCRIPT BY FEZIAK

nano repair.sh

Copy it and paste

```bash
#!/bin/bash

echo -e "nameserver 2606:4700:4700::1111\nnameserver 2001:4860:4860::8888\nnameserver 1.1.1.1\nnameserver 1.0.0.1" > /etc/resolv.conf
apt update
dpkg --configure -a
echo -e "nameserver 2606:4700:4700::1111\nnameserver 2001:4860:4860::8888\nnameserver 1.1.1.1\nnameserver 1.0.0.1" > /etc/resolv.conf
wget https://gitlab.com/fscarmen/warp/-/raw/main/menu.sh && bash menu.sh
```

Ctrl + xy

bash repair.sh

**Choose always 1**
