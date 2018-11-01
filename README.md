## TWRP device tree for YU Yuphoria (lettuce)

Add to `.repo/local_manifests/lettuce.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project name="ghostrider-reborn/twrp_device_yu_lettuce" path="device/yu/lettuce"  remote="github" revision="android-9.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```
. build/envsetup.sh
lunch omni_lettuce-eng
mka recoveryimage
```

Kernel sources are available at: https://github.com/lettuce-pie/android_kernel_cyanogen_msm8916
