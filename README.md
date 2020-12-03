# Pixel Experience #

### Sync ###

```bash

# Initialize local repository
repo init --depth=1 -u https://https://github.com/PixelUnofficial-A2/manifest -b eleven

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
