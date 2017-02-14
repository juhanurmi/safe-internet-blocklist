# safe-internet-blocklist

Example how to block some malware, spyware, user tracking, stupid or otherwise harmful content.

This is for yourself if you need to limit some harmful sites.

Edit this block list as you like and use it:

```sh
sudo cp /etc/hosts /etc/hosts.backup
sudo cp hosts /etc/hosts
```

I recommend using this:

[Another hosts block project](https://github.com/StevenBlack/hosts)

```sh
wget -O steven_hosts https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts
or
wget -O steven_hosts https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/fakenews-gambling-porn-social/hosts
cat head_of_hosts > hosts
grep -v "255\.255\.255\.255\|127\.0\.0\.1\|::1" steven_hosts >> hosts
```
