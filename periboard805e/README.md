# Periboard 805 ergo

This foldable bluetooth keyboard has a great travel size/weight but one big issue:
Using <kbd>ESC</kbd> requires <kbd>Fn</kbd> + <kbd>Shift</kbd> modifiers, which is a pain when using e.g. vim.
This custom layout simply swaps the ESCAPE, GRAVE and HOME keys.

## Android

See https://source.android.com/docs/core/interaction/input/key-layout-files

Make sure to get rooted adb and rw-mounted system:

```
adb root
adb shell mount -o remount,rw /
```

Push the file:

```
adb push Vendor_04e8_Product_7021_Version_011b.kl /system/usr/keylayout/
```

Make system ro again:

```
adb shell mount -o remount,ro /
```
