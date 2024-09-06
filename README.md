# AospEnhanced #

## Getting started ##

To get started with Android/AospEnhanced, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

## Download the source code ##

Initialize local repository
```bash
repo init -u https://github.com/AospEnhanced/android_manifest -b fifteen
```

You can shallow clone the source code if you have storage and internet limitiations
```bash
repo init -u https://github.com/AospEnhanced/android_manifest -b fifteen --depth=1
```

Sync the source
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

## Start Building ##

Set up environment
```bash
$ . build/envsetup.sh
```

Choose a target
```bash
$ lunch aosp_$device-ap3a-userdebug
```

Build the code
```bash
$ mka bacon -jX
```
