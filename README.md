# WypierdalajOS

### Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/WypierdalajOS/platform_manifest -b 12.1
# Sync
repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```

### Build ###

```bash
# Set up environment
$ . build/envsetup.sh
# Choose a target
$ lunch wypierdalaj_$device-userdebug
# Build the code
$ mka bacon -jX
```
