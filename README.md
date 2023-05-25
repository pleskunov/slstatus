# slstatus

## Description
This is a personal, experimental build of [slstatus](https://tools.suckless.org/slstatus/).
It is a vanilla slstatus with custom settings. No patches applied.

## Requirements
Currently slstatus works on FreeBSD, Linux and OpenBSD.
In order to build slstatus you need the Xlib header files.

- For volume percentage on Linux the kernel module `snd-mixer-oss` must be
  loaded.
- For volume percentage on FreeBSD, `sndio` must be installed.

In addition, you will need to install the scripts from `custom-modules` to your `$PATH`, [lm_sensors](https://hwmon.wiki.kernel.org/lm_sensors) and [Roboto Mono Nerd Fonts](https://github.com/ryanoasis/nerd-fonts/blob/master/patched-fonts/RobotoMono) family installed.

## Installation
```bash
git clone https://github.com/pleskunov/slstatus.git
cd slstatus
doas make clean install
```
## Configuration
slstatus can be customized by creating a custom config.h and (re)compiling the source code.
