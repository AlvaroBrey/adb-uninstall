# adb-uninstall

This is a bash script that uses [`fzf`](https://github.com/junegunn/fzf) to let you easily uninstall multiple apps over [ADB](https://developer.android.com/studio/command-line/adb).

![Demo GIF](res/demo.gif)

## Features

* Uninstall any user-installed (non-system) app from any connected device.
* Allows for selection of multiple apps.
* If more than one device is connected by ADB, will let you choose which one to uninstall from.
* Retrieves app names from the Google Play website to show a more user-readable name (not just package name)

## Requirements

`fzf` and `adb` must be properly installed and configured, and must be present in your `PATH`.

MacOS compatibility: install `sed` and `curl` from Homebrew.
The default versions probably won't work.

## Usage

Simply [download the script](https://raw.githubusercontent.com/alvarobrey/adb-uninstall/master/adb-uninstall) or clone this repository and run `adb-uninstall`.

Use the directional keys to navigate. Use the <kbd>TAB</kbd> key to select multiple packages if you so wish, and then press <kbd>ENTER</kbd> to proceed.

The script will show you the selected packages and will prompt for confirmation.

## License

This project is published under the [MIT License](LICENSE.txt).
