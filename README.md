# Project Blaze #
![20220304_195037](https://user-images.githubusercontent.com/87426352/156781124-0dec9231-9d4c-4b66-a8e8-036d1ced5c2e.png)
###Sync###

```bash

# Initialize local repository
repo init -u https://github.com/ProjectBlaze/manifest -b twelve

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
