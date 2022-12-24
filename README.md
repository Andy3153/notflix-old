<!-- vim: set fenc=utf-8 ts=2 sw=0 sts=0 sr et si tw=0 fdm=marker fmr={{{,}}}: -->
<h1 align="center">notflix-old</h1>
<p align="center">f@#k netflix use notflix a tool which search magnet links and stream it with webtorrent</p>

<p align="center">
<img src="./preview.gif" alt="Video Preview" width="500px">
</p>

## Why the fork?
I liked the old version of Notflix more and I wanted to get it back up and running.
Then, I realised I changed a lot of things and I decided to fork it and publish it.

## How does this work?

This is a shell script. It scrapes 1337x and gets the magnet link.
After this it uses [webtorrent](https://webtorrent.io/) to stream the video from the magnet link.
For scraping, the script uses simple gnu utils like sed, awk, paste, cut.


## Dependencies (in Arch Linux package names):
- coreutils
- curl
- dmenu
- gawk
- libnotify
- mpv
- sed
- webtorrent-cli

## Installation

### AUR package (coming soon)

### Manual method (not recommended)
Save the script in a folder that is inside your **$PATH** and give it execute permissions.

##### Example:
```sh
$ sudo curl -sL "https://raw.githubusercontent.com/Andy3153/notflix-old/master/notflix" -o /usr/local/bin/notflix
$ sudo chmod +x /usr/local/bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your **$PATH**, for example `sudo rm -f /usr/local/bin/notflix.

## TODO:
- [ ] Create AUR PKGBUILD
- [ ] Add support for more menus (?)

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).

