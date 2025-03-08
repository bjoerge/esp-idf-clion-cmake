# ESP-IDF + CLion + CMake example

Bare minimum hello world project for using ESP-IDF with CLion and CMake.

It focuses on local isolation and does not require esp-idf to be installed globally or idf.py to be manually added to PATH.

### Prerequisites
- direnv (https://direnv.net/)
- The required software packages listed [in the official esp-idf get started guide](https://docs.espressif.com/projects/esp-idf/en/stable/esp32/get-started/linux-macos-setup.html#step-1-install-prerequisites)

```sh
git clone --recursive https://github.com/bjoerge/esp-idf-clion-cmake
cd esp-idf-clion-cmake
direnv allow
sh ./deps/esp-idf/install.sh
. ./deps/esp-idf/export.sh
```

You might also need to run the following command (see the official guide [here](https://docs.espressif.com/projects/esp-idf/en/stable/esp32/get-started/linux-macos-setup.html#:~:text=For%20macOS%20users%2C%20if%20an%20error%20like%20this%20is%20shown%20during%20any%20step%3A))
```sh
sudo /Applications/Python\ 3.13/Install\ Certificates.command
```

## CLion Integration
Using direnv and opening the project in CLion from the project root via the terminal (eg. `clion .`) should work out of the box.
