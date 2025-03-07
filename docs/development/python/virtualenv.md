---
title: Virtualenv
description: Cheat sheet for virtualenv. Python Virtual Environment - virtualenv. How to install and Use virtualenv with Python. virtualenv is a tool to create isolated Python environments.
template: comments.html
tags: [python, virtualenv, cheat-sheet]
---

# Virtualenv

## About Python Virtual Environment - **virtualenv**

**virtualenv** is a tool to create isolated Python environments. Since Python 3.3, a subset of it has been integrated into the standard library under the venv module.
Using **virtualenv** is very useful for creating isolated Python environments for your project,it will allow you installing Python packages and modules in a separate location from the rest of your host os without conflicting versions.

## Install virtualenv

In order to install virtualenv, we need to install [**pip**][pip-url]{target=\_blank}

```shell
sudo apt install python3-pip
```

Now we can install the **virtualenv** with **pip** command:

```shell
sudo pip3 install virtualenv
```

## Create a Virtual Environment

cd to your project directory and run the following command to create a virtual environment:

```shell
virtualenv venv
```

!!! note

    you can use any name insted of **venv**
    You can also use a Python interpreter of your choice

Example of creating a virtual environment with Python 2.7 environment:

```shell
virtualenv -p /usr/bin/python2.7 venv
```

## Activate the Virtual Environment

In order to use the virtual environment, we need to activate it:

```shell
source venv/bin/activate
```

To deactivate:

```shell
deactivate
```

## Check the Python Version in the Virtual Environment

In order to check the Python version in the virtual environment, we can run the following command then the virtual environment will is activated:

```shell
which python
```

The output should point to the Python interpreter in the virtual environment (**/venv/bin/python**).

<!-- appendices -->

[pip-url]: https://pip.pypa.io/en/stable/ 'pip.pypa.io'

<!-- end appendices -->
