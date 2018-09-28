# Node.js

[Node.js](https://nodejs.org/en/) is a JavaScript runtime built on Chrome's
V8 JavaScript engine.

### Installation

###### Via package manager

Node.js is available from the NodeSource Debian and Ubuntu binary
distributions repository.

```bash
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt install -y nodejs
```

To compile and install native addons from npm you may also need to
install build tools:

```bash
sudo apt install -y build-essential
```

###### Via nvm

Node Version Manager is a bash script used to manage multiple released
Node.js versions. It allows you to perform operations like install,
uninstall, switch version, etc.

To install or update nvm, you can use:

```bash
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```

To download, compile, and install the latest release of node, do this:

```bash
nvm install node # "node" is an alias for the latest version
```

To install a specific version of node:

```bash
nvm install 8.9.1 # or 10.10.0, 6.14.4, etc
```

Useful commands:

```console
nvm ls                      # list installed Node version
nvm ls-remote               # list all the Node versions you can install
nvm alias default 10.11.0   # set the 10.11.0 version as the default Node
```

See the [documentation](https://github.com/creationix/nvm#usage) for more
examples.

### npm

[npm](https://docs.npmjs.com/) is a package manager for the JavaScript
programming language.

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
