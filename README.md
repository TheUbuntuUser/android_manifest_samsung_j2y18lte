# AncientOS ten webbo

### How to build ###

```bash
# Create dirs
$ mkdir ancient ; cd ancient

# Init repo
$ repo init --depth=1 -u https://github.com/Ancient-Lab/manifest -b ten-weeabo

# Clone my local repo
$ git clone https://github.com/TheUbuntuUser/android_manifest_samsung_j2y18lte.git -b ancient-10 .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh && lunch ancient_j2y18lte-userdebug && mka bacon -j`nproc`
```

## Credits
2021 @Astrako
