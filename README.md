# LineageOS 18.1

### How to build ###

```bash
# Create dirs
$ mkdir lineage ; cd lineage

# Init repo
$ repo init --depth=1 -u https://github.com/LineageOS/android.git -b lineage-18.1

# Clone my local repo
$ git clone https://github.com/TheUbuntuUser/android_manifest_samsung_j2y18lte.git -b lineage-18.1 .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh && lunch lineage_j2y18lte-userdebug && mka bacon -j`nproc`
```

## Credits
2021 @Astrako
