# SDKMAN

[SDKMAN!](https://sdkman.io/) is a tool for managing parallel versions of
multiple Software Development Kits. It provides a convenient Command Line
Interface (CLI) and API for installing, switching, removing and listing
Candidates.

## Installation

To install:

```bash
curl -s "https://get.sdkman.io" | bash
```

and follow the instruction to load SDKMAN! automatically.

## Usage

To list all available versions of Java:

```bash
sdk list java
```

To install specific versions:

```bash
sdk install java 9.0.7-zulu
sdk install java 7.0.211-zulu
```

To see what is currently in use:

```bash
sdk current java
```
