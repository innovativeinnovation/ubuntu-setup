# npm

[npm](https://docs.npmjs.com/) is a package manager for the JavaScript
programming language.

## Installation

The nodejs package contains the nodejs binary as well as npm, so you don't
need to install npm separately.

## Usage

To check npm version:

```bash
npm -v
```

To install a package:

```bash
npm i <package> # locally
npm i -g <package> # globally
```

To remove a package:

```bash
npm uninstall <package> # locally
npm uninstall -g <package> # globally
```

To update all or a particular package:

```bash
npm update [-g] [<package>]
```

To find outdated packages:

```bash
npm outdated [-g]
```

To see what's installed:

```bash
npm list [-g]
```
