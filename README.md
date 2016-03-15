# Mac-Stuff

## When `ping` returns 'cannot resolve, unknown host'

    sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.discoveryd.plist
    sudo launchctl load -w /System/Library/LaunchDaemons/com.apple.discoveryd.plist
[Details](http://apple.stackexchange.com/questions/26616/dns-not-resolving-on-mac-os)
