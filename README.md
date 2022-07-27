# OrangeFox Recovery Project

### How to build ###

```bash
# Create dirs
$ mkdir ofox ; cd ofox

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_7.1

# Clone j6lte repo
$ git clone https://github.com/TheUbuntuUser/orangefox_device_j2y18lte.git -b fox_7.1 device/samsung/j2y18lte

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ source build/envsetup.sh && lunch omni_j2y18lte-eng && mka recoveryimage -j16
```

## Credits
2019 @Astrako
