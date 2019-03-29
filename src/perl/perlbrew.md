# Perlbrew

[Perlbrew](https://perlbrew.pl/) is an admin-free perl installation
management tool.

## Installation

To install:

```bash
curl -L https://install.perlbrew.pl | bash
```

and follow the instruction to load Perlbrew automatically.

## Usage

To install specific versions:

```bash
perlbrew install 5.28.0
perlbrew install 5.14.4
```

To show installed versions:

```bash
perlbrew list
```

To run `myprogram.pl` against all installations of perl, especially helpful
when running tests:

```bash
perlbrew exec perl myprogram.pl
```
