# CPAN

[CPAN](https://www.cpan.org/) is the Comprehensive Perl Archive Network,
a large collection of Perl software and documentation.

## Installation

Ubuntu 22.04 ship with CPAN installed by default.

To compile and install package from CPAN you may also need to
install build tools:

```bash
sudo apt install -y build-essential
```

## Usage

To check CPAN version:

```bash
cpan -v
```

To install a package:

```bash
cpan install <package>
```
