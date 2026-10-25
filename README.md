# 🎬 mpv-android-custom (with `libmysofa` / `sofalizer`)

This repository is a custom fork of [mpv-android](https://github.com/mpv-android/mpv-android) featuring a custom-built `libmpv.so` **bundled with `libmysofa`**. 

Unlike the standard release, this build allows you to play movies and videos with multichannel audio (5.1, 7.1, etc.) while rendering them into **binaural stereo surround sound in real-time** using FFmpeg's `sofalizer` audio filter.

> 💡 **Want offline rendering instead?** If your device struggles with real-time processing or you want to permanently bake the binaural audio + AutoEQ into your file, check out [My-SofaLizeR](https://github.com/WinterFarmer/My-SofaLizeR).

---

## ✨ What's Different in This Fork?

- **`libmysofa` Bundled:** Built directly into `libmpv.so`, enabling full support for `.sofa` HRTF datasets.
- **Real-Time Spatial Audio:** Enjoy 3D binaural surround sound on the fly while watching movies without pre-rendering the video file.

---

## 🚀 How to Setup & Use `sofalizer`

Follow these steps to enable real-time HRTF binaural rendering in the app:

### 1. Place Your `.sofa` File into the App Directory
Download your preferred HRTF `.sofa` profile (e.g., from [sofaconvention.org](https://www.sofaconvention.org/)) and move/copy it into the `mpv-android` app data folder:

```text
/storage/emulated/0/Android/data/is.xyz.mpv/files/
