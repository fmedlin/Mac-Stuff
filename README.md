# Mac-Stuff

## Keyboard Shortcuts

This is a really nice collection:

[Dan Rodney's Mac Keyboard Shortcuts](https://www.danrodney.com/mac/)

## When `ping` returns 'cannot resolve, unknown host'

    $ sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.discoveryd.plist
    $ sudo launchctl load -w /System/Library/LaunchDaemons/com.apple.discoveryd.plist
[Details](http://apple.stackexchange.com/questions/26616/dns-not-resolving-on-mac-os)

## When you need `lsusb` on OSX

    $ brew update && brew tap jlhonora/lsusb && brew install lsusb
    $ lsusb
    Bus 020 Device 004: ID 05ac:8290 Apple Inc. Bluetooth USB Host Controller
    Bus 000 Device 001: ID 1d6b:IWPT Linux Foundation USB 3.0 Bus

or:

    $ ioreg -p IOUSB -l -w 0

[Details](http://stackoverflow.com/questions/17058134/is-there-an-equivalent-of-lsusb-for-os-x)
