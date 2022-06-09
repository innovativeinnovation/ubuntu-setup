# rbenv

[rbenv](https://github.com/rbenv/rbenv) is a Ruby Version Management tool
and lets you easily switch between multiple versions of Ruby.

## Installation

Requirements:

```bash
sudo apt install autoconf bison build-essential libssl-dev libyaml-dev \
libreadline6-dev zlib1g-dev libncurses5-dev libffi-dev libgdbm6 libgdbm-dev
```

To install:

```bash
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/HEAD/bin/rbenv-installer | bash
```

and follow the instruction to load rbenv automatically.

## Usage

To list all available versions of Ruby:

```bash
rbenv install -l
```

To install specific versions:

```bash
rbenv install 2.6.10
rbenv install 2.7.6
```

To show installed versions:

```bash
rbenv versions
```
