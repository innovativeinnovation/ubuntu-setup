# Ada

[Ada](https://www.adacore.com/about-ada) is a structured, statically typed,
imperative, and object-oriented high-level computer programming language. It
has built-in language support for design-by-contract, extremely strong typing,
explicit concurrency, tasks, synchronous message passing, protected objects,
and non-determinism. Ada improves code safety and maintainability by using
the compiler to find errors in favour of runtime errors.

## Installation

To install Ada:

```bash
sudo apt install gnat
```

## Usage

To check GNAT version:

```bash
gnat compile --version
```

To compile a program:

```bash
gnatmake <program>.adb
```

To delete files produced by the compiler, binder and linker:

```bash
gnatclean <program>
```
