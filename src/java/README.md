# Java

[Java](https://www.java.com) is a general-purpose computer-programming
language that is concurrent, class-based, object-oriented, and specifically
designed to have as few implementation dependencies as possible.

### Installation

###### Via package manager

To install Open JDK version 11:

```bash
sudo apt install openjdk-11-jdk
```

To install Open JDK version 8:

```bash
sudo apt install openjdk-8-jdk
```

To set default Java version manually:

```bash
sudo update-alternatives --config java
```

###### Via SDKMAN!

[SDKMAN!](https://sdkman.io/) is a tool for managing parallel versions of
multiple Software Development Kits. It provides a convenient Command Line
Interface (CLI) and API for installing, switching, removing and listing
Candidates.

To install:

```bash
curl -s "https://get.sdkman.io" | bash
```

and follow the instruction to load SDKMAN! automatically.

To list all available versions of Java:

```bash
sdk list java
```

To install specific versions:

```bash
sdk install java 9.0.7-zulu
sdk install java 7.0.191-zulu
```

To see what is currently in use:

```bash
sdk current java
```
