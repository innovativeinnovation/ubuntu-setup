# Node.js

[Node.js](https://nodejs.org/en/) is a JavaScript runtime built on Chrome's
V8 JavaScript engine.

## Installation

Node.js is available from the NodeSource Debian and Ubuntu binary
distributions repository.

```bash
curl -sL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
```

To compile and install native addons from npm you may also need to
install build tools:

```bash
sudo apt install -y build-essential
```

## Usage

To check Node.js version:

```bash
node -v
```

To view documentation:

```bash
man node
```
