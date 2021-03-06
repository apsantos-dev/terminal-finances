# Terminal Finances

This software is suitable for those who want to have control of their personal accounts in an easy and simple way. Available for Linux and Windows.

<!-- Badges section here. -->
[![License][license-img]][license-ln]
[![CONTRIBUTING][contributing-img]][contributing-ln]
[![GitHub stars][github-stars-img]][github-stars-ln]
[![GitHub forks][github-forks-img]][github-forks-ln]

---

## ![Terminal Finances - Personal Financial Management](terminal-finances.png) Terminal Finances - Personal Financial Management

![Terminal Finances running](screenshot.png)

---

## Installation

If you want to use Terminal Finances without compiling choose one of the options below to download:

- [AppImage Linux x86_64](https://github.com/terroo/terminal-finances/releases/download/v1.0.0/Terminal_Finances-x86_64.AppImage)

How to install:

```sh
wget https://github.com/terroo/terminal-finances/releases/download/v1.0.0/Terminal_Finances-x86_64.AppImage
chmod +x Terminal_Finances-x86_64.AppImage
./Terminal_Finances-x86_64.AppImage
```

Alternatively, you can use the [app-get](https://github.com/terroo/app-get). What makes it different is that it creates an icon on your Dashboard and makes it easier to access and update or remove. Example:

```sh
app-get terminal-finances
```

- [Windows 10 64-bit](https://github.com/terroo/terminal-finances/releases/download/v1.0.0/TerminalFinances_installer_Win10_64.rar)
  - Download it by [clicking on this link](https://github.com/terroo/terminal-finances/releases/download/v1.0.0/TerminalFinances_installer_Win10_64.rar)
  - Unzip the **.rar** file
  - Double-click the installation file to install
  - And after the installation is finished, access the program through the start menu

---

## Building the Terminal Finances

First of all you will need the dependencies:

- [qmake](https://en.wikipedia.org/wiki/Qmake)
- [g++](https://gcc.gnu.org/)
- [GNU Make](https://www.gnu.org/software/make/)
- libQt5Widgets
- libQt5Gui
- libQt5Core
- libQt5Sql
- libQt5PrintSupport

For example, on Ubuntu, Linux Mint, Debian and derivatives the command would be:

```sh
sudo apt install qmake g++ make libqt5widgets5 libqt5gui5 libqt5core5a libqt5sql libqt5printsupport5
```

Then clone the repository and compile as follows:

```sh
git clone https://github.com/terroo/terminal-finances
cd terminal-finances
qmake -qt=qt5 src/TerminalFinances.pro
make
sudo make install
```

---

## Use

I am still developing the Wiki, but while it is not ready you can see how to use it through this video:

> Activate subtitles and choose the language according to yours.

## <https://youtu.be/BF809OoXfjM>

If you find a bug or want a feature to be implemented for the new versions use the [issues](https://github.com/terroo/terminal-finances/issues) to inform.

---

## Uninstall

> Compiled version

Clone the repository if you don't have:

```sh
cd terminal-finances
sudo make uninstall
```

> Windows

Access the Control Panel and Add/Remove Programs and uninstall

> app-get

- [app-get](https://github.com/terroo/app-get)/Linux

```sh
app-get --remove terminal-finances
```

---

### Change Log

All notable changes to this project will be documented in this file [CHANGELOG.md][changelog-ln].

_Stable release version:_

[![Release][release-img]][release-ln]

---

### Contributing

You can contribute by opening an issue or creating a pull request.

_See details on contributing to this project at:_

[![CONTRIBUTING][contributing-img]][contributing-ln]

---

## License

This project is licensed under "**GNU GPLv3**".

_See license details at:_

[![License][license-img]][license-ln]

---

<!-- links -->
[changelog-ln]: CHANGELOG.md "Click here to open the file"
[contributing-img]: https://img.shields.io/badge/terminal_finances-CONTRIBUTE-orange.svg?style=flat-square
[contributing-ln]: CONTRIBUTING.md "Contribute to make this project even better"
[github-stars-img]: https://img.shields.io/github/stars/terroo/terminal-finances.svg?style=social&label=Star
[github-stars-ln]: https://github.com/terroo/terminal-finances/stargazers "See who likes this design = ]"
[github-forks-img]: https://img.shields.io/github/forks/terroo/terminal-finances.svg?style=social&label=Fork
[github-forks-ln]: https://github.com/terroo/terminal-finances/fork "Click to view Star details of this project"
[license-img]: https://img.shields.io/badge/license-GNU_GPLv3-blue.svg?style=flat-square
[license-ln]: LICENSE "GNU GPLv3"
[release-img]: https://img.shields.io/github/release/terroo/terminal-finances.svg?style=flat-square
[release-ln]: https://github.com/terroo/terminal-finances/releases "See all versions of this project"
