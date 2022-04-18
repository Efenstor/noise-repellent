# noise-repellent

An suite of lv2 plugins for noise reduction that uses [libspecbleach](https://github.com/lucianodato/libspecbleach) C library.

[![master](https://github.com/lucianodato/noise-repellent/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/lucianodato/noise-repellent/actions/workflows/build.yml)
[![DEVELOPMENT](https://github.com/lucianodato/noise-repellent/actions/workflows/build.yml/badge.svg?branch=DEVELOPMENT)](https://github.com/lucianodato/noise-repellent/actions/workflows/build.yml)

## Features

* Adaptive noise reduction plugin for low latency voice denoise
* Manual noise capture based plugin for customizable noise reduction
* Adjustable Reduction and many other parameters to tweak the reduction
* Option to listen to the residual signal
* Soft bypass
* Noise profile saved with the session

## Install

Binaries for most platforms are provided with Github release. Just extract the adequate zip file for your platform to your [lv2 plugins folder](https://lv2plug.in/pages/filesystem-hierarchy-standard.html)

If you wish to compile yourself and install this plug-in you will need the a C compiling toolchain, LV2 SDK, Meson build system, ninja compiler, git and fftw3 library.

Installation:

```bash
  git clone https://github.com/lucianodato/noise-repellent.git
  cd noise-repellent
  meson build --buildtype=release --prefix=/usr --libdir=lib (your-os-appropriate-location-fullpath)
  ninja -C build -v
  sudo ninja -C build install
```

Noise-repellent is on Arch community at <https://www.archlinux.org/packages/community/x86_64/noise-repellent/>.

Noise-repellent is also available in KXStudios repositories <https://kx.studio/Repositories:Plugins>

## Use Instuctions

Please refer to project's wiki <https://github.com/lucianodato/noise-repellent/wiki>
