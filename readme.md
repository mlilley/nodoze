# NODOZE
Make corporate macs listen to your DisplaySleep setting.

## Install

Update plist paths as needed, adjust job interval (if necessary, currently runs every 10 minutes) then:
```
$ brew install moreutils
$ sudo cp local.nodoze.plist /Library/LaunchDaemons
$ sudo launchctl load -w /Library/LaunchDaemons/local.nodoze.plist
```

## Uninstall
```
$ sudo launchctl unload -w /Library/LaunchDaemons/local.nodoze.plist
$ sudo rm /Library/LaunchDaemons/local.nodoze.plist
```
