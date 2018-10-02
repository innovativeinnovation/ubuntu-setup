# Python

[Python](https://www.python.org/) is a flexible and versatile programming
language that can be leveraged for many use cases, with strengths in
scripting, automation, data analysis, machine learning, and back-end
development.

### Installation

###### Via package manager

Ubuntu 18.04 ship with both Python 3 and Python 2 pre-installed.

To install pip for Python 2 and Python 3:

```bash
sudo apt install -y python-pip python3-pip
```

###### Via pyenv

[pyenv](https://github.com/pyenv/pyenv) is a Python Version Management tool
and lets you easily switch between multiple versions of Python.

Requirements:

```bash
sudo apt install -y make build-essential libssl-dev zlib1g-dev libbz2-dev \
libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev \
xz-utils tk-dev libffi-dev liblzma-dev
```

To install:

```bash
curl -L https://github.com/pyenv/pyenv-installer/raw/master/bin/pyenv-installer | bash
```

and follow the instruction to load pyenv automatically.

To list all available versions of Python:

```bash
pyenv install --list
```

To install specific versions:

```bash
pyenv install 2.7.15
pyenv install 3.7.0
```

To show installed versions:

```bash
pyenv versions
```

### pip

[pip](https://pypi.org/project/pip/) is a package management system used to
install and manage software packages written in Python.

To install a package:

```bash
pip install <package>
```

To uninstall a package:

```bash
pip uninstall <package>
```

To upgrade a package:

```bash
pip install --upgrade <package>
```

To output installed packages:

```bash
pip freeze
```
