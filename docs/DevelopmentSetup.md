# Development Setup

## Introduction

This page describes how to set up a development environment, and other
information useful for developers to be aware of.

## Prerequisites

The following instructions assume that "pyenv" and "pyenv-virtualenv" are
installed to enable the setup of an isolated Python environment.

See the following for setup instructions:

* <https://github.com/pyenv/pyenv>
* <https://github.com/pyenv/pyenv-virtualenv>

Once "pyenv" and "pyenv-virtualenv" have been installed, install Python 3.7.10:

```
> pyenv install 3.7.10
```

## Installation for development

1) Clone the "preserve" Git repository:

```
> git clone git@github.com:umd-lib/preserve.git
```

2) Switch to the "caia" directory:

```
> cd preserve
```

3) Set up the virtual environment:

```
> pyenv virtualenv 3.7.10 preserve
> pyenv shell preserve
```

4) Run "pip install", including the "dev" and "test" dependencies:

```
> pip install -e .[dev,test]
```