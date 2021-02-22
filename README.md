# README
## Build Environment Setup for my CandyROMs 11 Development Projects

Setup the build environment following the usual AOSP/CandyROMs guide.

Setup your local sources using the CandyROMs sources as follows:

```
repo init -u git://github.com/LineageOS/android.git -b candy-11

```

```
git clone https://github.com/rajatgupta1998/local_manifests.git -b candy-11 .repo/local_manifests
```

Then to sync up:
```
repo sync --force-sync --no-tags --no-clone-bundle --optimized-fetch --prune -c -j$(nproc --all)
```

For building the final ROM zip:
```
. build/envsetup.sh && brunch candy_<device>-userdebug -j$(nproc --all)
```


For any assistance or dev support, feel free to drop an email or a message at XDA or Telegram.