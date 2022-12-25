<!-- vim: set fenc=utf-8 ts=2 sw=0 sts=0 sr et si tw=0 fdm=marker fmr={{{,}}}: -->
# notflix-old

<!-- {{{ Why the fork? -->
## Why the fork?
I liked the old version of Notflix more and I wanted to get it back up and running.
Then, I realised I changed a lot of things and I decided to fork it and publish it.
<!-- }}} -->

<!-- {{{ How does this work? -->
## How does this work?
The scrpt scrapes 1337x and gets a magnet link.
After this, it uses [webtorrent](https://webtorrent.io/) to stream the video from the magnet link.
For scraping, the script uses simple GNU utils like sed, awk, paste, cut.
<!-- }}} -->

<!-- {{{ Dependencies -->
## Dependencies (in Arch Linux package names):
- coreutils
- curl
- dmenu
- gawk
- grep
- libnotify
- mpv
- sed
- webtorrent-cli
<!-- }}} -->

<!-- {{{ Installation -->
## Installation

<!-- {{{ AUR package -->
### AUR package
The AUR package is available [here](https://aur.archlinux.org/packages/notflix-old). You can just use your favourite AUR helper to install it.

##### Example:
```sh
$ paru -S notflix-old
```
<!-- }}} -->

<!-- {{{ Manual method -->
### Manual method (not recommended)
Save the script in a folder that is inside your **$PATH** and give it execute permissions.

##### Example:
```sh
$ sudo curl -sL "https://raw.githubusercontent.com/Andy3153/notflix-old/master/notflix" -o /usr/local/bin/notflix
$ sudo chmod +x /usr/local/bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your **$PATH**, for example `sudo rm -f /usr/local/bin/notflix.
<!-- }}} -->
<!-- }}} -->

<!-- {{{ TODO -->
## TODO:
- [x] Create AUR PKGBUILD
- [ ] Add desktop entry (?)
- [ ] Add support for more menus (?)
<!-- }}} -->

<!-- {{{ Credits -->
## Credits:
- [Bugswriter](https://github.com/Bugswriter), the original creator of [Notflix](https://github.com/Bugswriter/notflix)
<!-- }}} -->

<!-- {{{ License -->
## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).
<!-- }}} -->
