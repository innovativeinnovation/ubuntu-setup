# pip

[pip](https://pypi.org/project/pip/) is a package management system used to
install and manage software packages written in Python.

## Installation

To install pip for Python 2 and pip3 for Python 3:

```bash
sudo apt install -y python-pip python3-pip
```

## Usage

To install a package:

```bash
pip install <package>
pip3 install <package>
```

To uninstall a package:

```bash
pip uninstall <package>
pip3 uninstall <package>
```

To upgrade a package:

```bash
pip install --upgrade <package>
pip3 install --upgrade <package>
```

To output installed packages:

```bash
pip freeze
pip3 freeze
```
