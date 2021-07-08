# Pixel Experience #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/PixelExp-Project/manifest -b eleven

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```

### Submitting Patches ###

Patches are always welcome! Please submit your patches to our Gerrit.

[Gerrit push guide](https://wiki.pixelexperience.org/help/submit-patch/)
