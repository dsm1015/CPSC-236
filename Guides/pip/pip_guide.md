# Pip Guide for Python Packages

Video guide: https://sru.mediaspace.kaltura.com/media/t/1_0hkoy1ly

Pip is the Python Package Installer. It allows you to install and manage additional libraries and dependencies that are not distributed as part of the standard library. This guide covers the basics of using `pip` to install packages, list installed packages, and generate a `requirements.txt` file for your projects.

## Installing Packages with Pip

To install a package using `pip`, use the `install` command followed by the name of the package. For example, to install the `pygame` library, you would use the following command:

`pip install pygame`

### Installing Specific Versions

To install a specific version of a package, use the `==` operator followed by the version number. For example, to install version 2.5.2 of `pygame`, you would use:

`pip install pygame==2.5.2`

### Installing Packages from a Requirements File

To install multiple packages at once, you can list them in a `requirements.txt file`, one package per line, and then tell `pip` to install all of them using the `-r` flag:

`pip install -r requirements.txt`

## Listing Installed Packages

To list all the packages installed in your current environment, use the `list` command:

`pip list`

This command will display a list of installed packages along with their versions.

## Freezing Installed Packages

To generate a `requirements.txt` file containing all the installed packages in your environment along with their exact versions, use the `freeze` command:

`pip freeze > requirements.txt`

This will create (or overwrite) a `requirements.txt` file in your current directory with the output from `pip freeze`.

### What pip freeze Outputs

The `pip freeze` command outputs a list of package specifications in the format `package==version`, which is suitable for use in a `requirements.txt` file. This file can then be used with `pip install -r requirements.txt` to replicate the environment elsewhere.

## Upgrading Packages

To upgrade an installed package to the latest version, use the `install` command with the `--upgrade` (or `-U`) flag:

`pip install --upgrade pygame`

This will upgrade the requests package to its latest version, along with its dependencies.

## Uninstalling Packages

To remove a package installed with `pip`, use the `uninstall` command followed by the name of the package:

`pip uninstall pygame`

You will be prompted to confirm the uninstallation.