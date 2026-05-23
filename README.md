# SkiaSharp.Static

Static library of Skia Sharp for Avalonia UI

For **Skia 3**, you must use with **Avalonia 12**.

A sample project here: <https://github.com/peaceshi/Avalonia-NativeAOT-SingleFile>

## Linux (NativeAOT)

The `2ndLAB.SkiaSharp.Static.Linux` package supports `linux-x64` and `linux-arm64`. The static libraries link against fontconfig and freetype dynamically — the consumer machine must have those installed.

On the build/publish machine:

```bash
sudo apt-get install -y libfontconfig1-dev libfreetype-dev
```

On the deployment target:

```bash
sudo apt-get install -y libfontconfig1
```

`libfreetype.so.6` is pulled in by `libfontconfig1`, so no separate runtime package is needed for freetype.
