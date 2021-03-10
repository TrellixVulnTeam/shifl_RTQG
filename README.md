# SHIFL
Spark-Hadoop Installer For Unix

![](https://img.shields.io/badge/system-macOS%7CLinux%7CFreeBSD-green)

[![Python](https://img.shields.io/pypi/pyversions/shifl.svg?logo=python&logoColor=white)](https://pypi.org/project/shifl)

This package uses Python to download and unpack a pre-built version of Spark/Hadoop from Apache.
Its primary use-case is simplifying unattended installs where the user wants "the latest available version" of these tools.

## Features

* download Spark/Hadoop release from Apache.
* unpack the tarball to a target directory on your local system.

## Installation

First you'll need to install `shifl` using pip: `pip install shifl`. **Note** this requires `Python >= 3.6`.

## Common usage examples

### Versions

```
USAGE
  shifl versions [--latest]

OPTIONS
  --latest               Show only the latest available version

GLOBAL OPTIONS
  -h (--help)            Display this help message
  -q (--quiet)           Do not output any message
  -v (--verbose)         Increase the verbosity of messages: "-v" for normal output, "-vv" for more verbose output and "-vvv" for debug
  -V (--version)         Display this application version
  --ansi                 Force ANSI output
  --no-ansi              Disable ANSI output
  -n (--no-interaction)  Do not ask any interactive question
```

### Install

```
USAGE
  shifl install [--latest] [--spark <...>] [--hadoop <...>] [--target <...>]

OPTIONS
  --latest               Use the latest available version
  --spark                Spark version (default: "any")
  --hadoop               Hadoop version (default: "any")
  --target               Directory to install into (defaults to current working directory) (default: "cwd")

GLOBAL OPTIONS
  -h (--help)            Display this help message
  -q (--quiet)           Do not output any message
  -v (--verbose)         Increase the verbosity of messages: "-v" for normal output, "-vv" for more verbose output and "-vvv" for debug
  -V (--version)         Display this application version
  --ansi                 Force ANSI output
  --no-ansi              Disable ANSI output
  -n (--no-interaction)  Do not ask any interactive question
```