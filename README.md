# throw_and_liberty

VR arena game for PICO standalone headsets, built with Unreal Engine 5.6 (Blueprint project).

## Requirements

- Unreal Engine 5.6.x
- Git with Git LFS: run `git lfs install` before cloning, otherwise `.uasset`, `.umap` and plugin DLLs stay as pointer files
- The PICO OpenXR plugin is already in `Plugins/`, nothing to install

## Packaging for the headset (Android)

Only needed to build an APK, not to work in the editor.

1. Visual Studio with the C++ toolchain (the PICO plugin is compiled for Android at packaging time)
2. Android Studio, then run `Engine\Extras\Android\SetupAndroid.bat` from the UE 5.6 install folder
3. Set the SDK, NDK and Java paths in `Project Settings > Platforms > Android SDK`
4. The Android package name (`com.p10.throwandliberty`) is already set in `Config/DefaultEngine.ini`, do not change it
