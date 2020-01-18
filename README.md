# montclair-pwa-android

This is a simple wrapper around the Montclair project at (https://montclair.line72.net/) using cordova and PWA Builder (pwabuilder.com) to generate a native Android app.

## Info

Copyright (c) Marcus Dillavou <line72@line72.net>
https://github.com/line72/montclair-pwa-android

## License

GPLv3

## Releases

Releases are automatically built by github actions and are uploaded as
a release. However, the releases are un-aligned and un-signed, so they
need to be manually fixed:

```
zipalign 4 montclair-pwa-android-1.0.2-2-release-unsigned.apk montclair-pwa-android-1.0.2-2-release.apk
apksigner sign --ks release-key.keystore --ks-key-alias montclair montclair-pwa-android-1.0.2-2-release.apk
```
