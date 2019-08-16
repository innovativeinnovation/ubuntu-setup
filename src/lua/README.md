# Lua

[Lua](https://www.lua.org/) is a powerful, efficient, lightweight, embeddable
scripting language. It supports procedural programming, object-oriented
programming, functional programming, data-driven programming, and data
description.

## Installation

To install Lua version 5.3:

```bash
sudo apt install lua5.3
```

To install Lua version 5.2:

```bash
sudo apt install lua5.2
```

## Configuration

Installing lua5.3 package does not provide alternative for lua-interpreter and
lua-compiler. You can add it with:

```bash
sudo update-alternatives --install /usr/bin/lua lua-interpreter /usr/bin/lua5.3 130 --slave /usr/share/man/man1/lua.1.gz lua-manual /usr/share/man/man1/lua5.3.1.gz

sudo update-alternatives --install /usr/bin/luac lua-compiler /usr/bin/luac5.3 130 --slave /usr/share/man/man1/luac.1.gz lua-compiler-manual /usr/share/man/man1/luac5.3.1.gz
```

To set default Lua interpreter version manually:

```bash
sudo update-alternatives --config lua-interpreter
```

To set default Lua compiler version manually:

```bash
sudo update-alternatives --config lua-compiler
```
