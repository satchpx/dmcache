# Setup a px caching device for a slower device or device pool

## Install the service
```
curl -s https://raw.githubusercontent.com/satchpx/dmcache/master/pxcache.service > /etc/systemd/system/pxcache.service
vi /etc/systemd/system/pxcache.service
<Replace dev1 and dev2 with the fast_device and slow_device respectively
systemctl daemon-reload
systemctl start pxcache
```
