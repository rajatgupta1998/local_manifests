# README
## Build Environment Setup for Moto G4 Plus LineageOS 15.1 Development

Setup the build environment following the usual AOSP/LineageOS guide.

Setup your local sources using the LineageOS and athene sources as follows:

```
repo init -u git://github.com/LineageOS/android.git -b lineage-15.1

```

```
git clone https://github.com/rajatgupta1998/local_manifests.git -b lineage-15.1 .repo/local_manifests
```

Then to sync up:
```
repo sync --force-sync --no-tags --no-clone-bundle --optimized-fetch --prune -c -j$(nproc --all)
```

For building the final ROM zip:
```
. build/envsetup.sh && brunch lineage_athene-userdebug -j$(nproc --all)
```



For any assistance or dev support, feel free to drop an email or a message at XDA or Telegram.