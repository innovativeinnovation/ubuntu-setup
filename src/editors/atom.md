# Atom

[Atom](https://atom.io/) is a free and open-source text and source code
editor with support for plug-ins written in Node.js, and embedded Git Control,
developed by GitHub.

## Installation

```bash
wget -qO- https://packagecloud.io/AtomEditor/atom/gpgkey | gpg --dearmor | sudo tee /usr/share/keyrings/atom.gpg
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/atom.gpg] https://packagecloud.io/AtomEditor/atom/any/ any main" | sudo tee /etc/apt/sources.list.d/atom.list
sudo apt update
sudo apt install atom
```

## Atom Package Manager (apm)

Atom Package Manager is bundled and installed automatically with Atom.

## Settings

These settings are all optional, consider them suggestions.

### Core Settings

* Allow Pending Pane Items -> Off

### Editor Settings

* Font Size -> 12px
* Show Invisibles -> On

## Themes

You can find your favorite themes on
[https://atom.io/themes](https://atom.io/themes).

UI Theme that I use:

* Seti UI - `apm install seti-ui`
  * Theme Color -> Pink
  * Compact Mode -> On

Syntax Theme that I use:

* Seti Syntax - `apm install seti-syntax`
  * Dynamic Theme -> On

## Packages

You can search packages on
[https://atom.io/packages](https://atom.io/packages).

Packages that I use:

* [atom-beautify](https://atom.io/packages/atom-beautify) - `apm install atom-beautify`
* [editorconfig](https://atom.io/packages/editorconfig) - `apm install editorconfig`
* [linter](https://atom.io/packages/linter) - `apm install linter`
* [teletype](https://atom.io/packages/teletype) - `apm install teletype`
