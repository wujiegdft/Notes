```sh
dd if=/dev/zero of=swapfile bs=1M count=1536
chmod 0600 swapfile
mkswap swapfile
swapon swapfile
free -m
echo ./swapfile swap swap defaults 0 0 >> /etc/fstab
```
