# pyenv

[pyenv](https://github.com/pyenv/pyenv) is a Python Version Management tool
and lets you easily switch between multiple versions of Python.

## Installation

Requirements:

```bash
sudo apt install -y make build-essential libssl-dev zlib1g-dev libbz2-dev \
libreadline-dev libsqlite3-dev wget curl llvm libncursesw5-dev \
xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```

To install:

```bash
curl https://pyenv.run | bash
```

and follow the instruction to load pyenv automatically.

## Usage

To list all available versions of Python:

```bash
pyenv install --list
```

To install specific versions:

```bash
pyenv install 2.7.18
pyenv install 3.7.0
```

To show installed versions:

```bash
pyenv versions
```
