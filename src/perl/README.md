# Perl

[Perl](https://www.perl.org/) is a high-level general-purpose, interpreted,
dynamic programming language including Perl 5 and Perl 6. Only Perl 5 is
detailed here for now.

### Installation

###### Via package manager

Ubuntu 18.04 ship with Perl 5.26 pre-installed.

###### Via Perlbrew

[Perlbrew](https://perlbrew.pl/) is an admin-free perl installation
management tool.

To install:

```bash
curl -L https://install.perlbrew.pl | bash
```

and follow the instruction to load Perlbrew automatically.

To install specific versions:

```bash
perlbrew install 5.28.0
perlbrew install 5.14.4
```

To show installed versions:

```bash
perlbrew list
```

### CPAN

[CPAN](https://www.cpan.org/) is the Comprehensive Perl Archive Network,
a large collection of Perl software and documentation.

To install a package:

```bash
cpan install <package>
```
