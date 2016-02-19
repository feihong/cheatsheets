# Ruby

## Installing gems that try to install binaries to /usr/bin

The best solution is to install to `/usr/local/bin` instead of `/usr/bin`.

```
sudo gem install -n /usr/local/bin cocoapods
```

Source: http://stackoverflow.com/questions/32810808/can-not-perform-pod-install-under-el-capitan-15a279b?lq=1
