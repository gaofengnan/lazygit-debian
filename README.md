![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/gaofengnan/lazygit-debian/total)
![GitHub Downloads (all assets, latest release)](https://img.shields.io/github/downloads/gaofengnan/lazygit-debian/latest/total)
![GitHub Release](https://img.shields.io/github/v/release/gaofengnan/lazygit-debian)
![GitHub Release Date](https://img.shields.io/github/release-date/gaofengnan/lazygit-debian)

<h1>
   <p align="center">
     <a href="https://lazygit.org/"><img src="https://github.com/gaofengnan/lazygit-debian/blob/main/lazygit-logo.png" alt="lazygit Logo" width="128" style="margin-right: 20px"></a>
     <a href="https://www.debian.org/"><img src="https://github.com/gaofengnan/lazygit-debian/blob/main/debian-logo.png" alt="Debian Logo" width="104" style="margin-left: 20px"></a>
     <br>lazygit for Debian
   </p>
</h1>
<p align="center">
 lazygit is a simple terminal UI for git commands.
</p>

# lazygit for Debian

> Fork of [dariogriffo/lazygit-debian](https://github.com/dariogriffo/lazygit-debian) (MIT); the original packaging is by Dario Griffo. Served at [deb.gaofn.xyz](https://deb.gaofn.xyz) for Debian 12 (bookworm) and 13 (trixie).

This repository contains build scripts to produce the _unofficial_ Debian packages
(.deb) for [lazygit](https://github.com/jesseduffield/lazygit/) hosted at [deb.gaofn.xyz](https://deb.gaofn.xyz)

Currently supported debian distros are:
- Bookworm
- Trixie
- Sid

This is an unofficial community project to provide a package that's easy to
install on Debian. If you're looking for the lazygit source code, see
[lazygit](https://github.com/jesseduffield/lazygit/).

## Install/Update

### The Debian way

```sh
sudo install -d -m 0755 /etc/apt/keyrings
sudo curl -fsSL https://deb.gaofn.xyz/deb.gaofn.xyz.gpg -o /etc/apt/keyrings/deb.gaofn.xyz.gpg
sudo curl -fsSL https://deb.gaofn.xyz/deb.gaofn.xyz.sources -o /etc/apt/sources.list.d/deb.gaofn.xyz.sources
# Debian 12 (bookworm): fetch deb.gaofn.xyz-bookworm.sources instead
sudo apt update
sudo apt install -y lazygit
```

### Manual Installation

1. Download the .deb package for your Debian version available on
   the [Releases](https://github.com/gaofengnan/lazygit-debian/releases) page.
2. Install the downloaded .deb package.

```sh
sudo dpkg -i <filename>.deb
```
## Updating

To update to a new version, just follow any of the installation methods above. There's no need to uninstall the old version; it will be updated correctly.

## Roadmap

- [x] Produce a .deb package on GitHub Releases
- [x] Set up a debian mirror for easier updates

## Disclaimer

- This repo is not open for issues related to lazygit. This repo is only for _unofficial_ Debian packaging.
