# QtApng
apng image plugin for Qt to support animated PNGs

## Features
Enable the usage of apng images with Qt. The plugin adds the apng format as a new format for any Qt application, and thus supports loading of apng images via `QMovie`, `AnimatedImage` and other types.

## Requirements
To build the plugin, libpng with the apng patch applied is required. By default the libpng provided by `pkg-config` is used for unix-like systems. If the library is not available, the project will compile a static library of libpng and embed it into the plugin. You can force this behaviour by running qmake with `CONFIG += libpng_static`

## Usage
Simply use the default Qt classes like `QImageReader`, `QMovie` etc. and open the apng files just like you would open normal images/animations (like gif files)

**Format Detection:**
Since the png format is already used by Qt, `*.png` files will **not** use the plugin. To load a png as animated, you can either rename the file to `*.apng`, or set the format explicitly

```cpp
QMovie movie("path/to/image.png", "apng");
```
