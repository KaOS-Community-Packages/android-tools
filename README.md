# Android Tools (Platform Tools)

#### [HOME](http://tools.android.com/) | [SOURCE](https://github.com/nmeum/android-tools)

### Install:

```
kcp -i android-tools
```
Android SDK Platform-Tools is a component for the Android SDK. It includes tools that interface with the Android platform, primarily `adb` and `fastboot`. Although `adb` is required for Android app development, app developers will normally just use the copy Studio installs. This download is useful if you want to use `adb` directly from the command-line and don't have Studio installed. (If you do have Studio installed, you might want to just use the copy it installed because Studio will automatically update it.) `fastboot` is needed if you want to unlock your device bootloader and flash it with a new system image. This package used to contain systrace, but that has been obsoleted in favor of Studio Profiler, gpuinspector.dev, or Perfetto.

Although some new features in `adb` and `fastboot` are available only for recent versions of Android, they're backward compatible, so you should only need the latest version of the SDK Platform-Tools and should file bugs if you find exceptions.

##### *This package might need `android-udev-rules` as dependency, can be obtained using `kcp -i android-udev-rules`*
##### *This package is a dependency for `scrcpy`*
