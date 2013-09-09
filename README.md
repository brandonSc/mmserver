# Modified Mobile Mouse Server for Linux

Use your iOS or Android device as a network mouse and keyboard for your Linux computer using [Mobile Mouse](http://www.mobilemouse.com/) and this software, which is a fork of [Mobile Mouse Server for Linux](http://sourceforge.net/projects/mmlinuxserver/) by Erik Lax. This fork by Jim DeVona is based on an [earlier fork](https://github.com/kiriakos/mmserver) by Kiriakos Krastillos.

## Modifications

- Revised mouse acceleration algorithm.
- Added support for horizontal scrolling.
- Added user-configurable scrolling speed limit.
- Added support for middle mouse button.
- Fixed numeric keypad input of numerals.
- Fixed keyboard input of capital letters and some other characters (hack).
- Other minor changes and simplifications.

## Installation

First, install prerequisite packages:

```sh
sh builddep.sh
```

Then, prepare the build directory:

```sh
mkdir build
cd build
cmake ..
```

Lastly, compile and install the software:

```sh
make
sudo make install
```

Invoke by running `mmserver` or by choosing *Mobile Mouse Server for Linux* from your system menu.

## Compatibility

Tested with version 2.7.1 of Mobile Mouse Pro for iOS. Other versions may or may not be compatible.

## License

This software is freely distributed under the terms of the [GNU General Public License, version 2.0](http://www.gnu.org/licenses/gpl-2.0.txt). See the `LICENSE` file for details.
