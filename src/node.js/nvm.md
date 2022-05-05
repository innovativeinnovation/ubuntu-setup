# nvm

Node Version Manager is a bash script used to manage multiple released
Node.js versions. It allows you to perform operations like install,
uninstall, switch version, etc.

## Installation

To install or update nvm, you can use:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

To download, compile, and install the latest release of node, do this:

```bash
nvm install node # "node" is an alias for the latest version
```

To install a specific version of node:

```bash
nvm install 16.13.0 # or 12.22.7, 14.0.0, etc
```

## Usage

To check nvm version:

```bash
nvm --version
```

Useful commands:

```console
nvm ls                      # list installed Node version
nvm ls-remote               # list all the Node versions you can install
nvm alias default 16.13.0   # set the 16.13.0 version as the default Node
```

See the [documentation](https://github.com/creationix/nvm#usage) for more
examples.
