Nvidia drivers patch for Windows
================================

This patch removes restriction on maximum number of simultaneous NVENC video encoding sessions imposed by Nvidia to consumer-grade GPUs.

Windows support is experimental.

Requirements:
- Win10 x64
- NVENC-compatible GPU (https://developer.nvidia.com/video-encode-decode-gpu-support-matrix#Encoder)
- Nvidia driver. Patch availible for:
  - [417.35](https://uk.download.nvidia.com/Windows/417.35/417.35-desktop-win10-64bit-international-whql-rp.exe)

## Step-by-Step guide

1. Download and install latest Nvidia driver supported by this patch.
2. Download latest [Win\_1337\_Apply\_Patch tool](https://github.com/Deltafox79/Win_1337_Apply_Patch/releases).
3. Locate in this directory and download corresponding patch for your OS and driver version.
4. Apply patch to corresponding file in `%WINDIR%\system32\` with the Win\_1337\_Apply\_Patch tool. File name of patched object is specified in first line of .1337 patch.

E.g, for 64bit Windows 10 running driver version 417.35 use `win10_x64/417.35/nvcuvid.1337` against `C:\WINDOWS\system32\nvcuvid.dll`.

## See also

* Genesis in [related issue](https://github.com/keylase/nvidia-patch/issues/9).
* [How to make Plex work with new limits](https://github.com/keylase/nvidia-patch/issues/9#issuecomment-452096166).