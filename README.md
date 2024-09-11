## Notes for building the MacOS application

1. You need [Homebrew](https://brew.sh).
2. Install WXWidgets with `brew install wxwidgets`.
3. Once installed, run `brew info wxwidgets` to see the specific path to where it is installed on _your_ Mac. It will likely say "Installed `/opt/homebrew/Cellar/wxwidgets/3.2.6` — but it could be different. Make a note of this path.
4. Look at line 15 of the Makefile in this repo... and change the path to `/bin/wx-widget-config` as needed. i.e. `WXCONFIG = [PATH/TO/THE/WIDGETS]/bin/wx-config`
5. Run the `make` command in the project directory to build the app.
