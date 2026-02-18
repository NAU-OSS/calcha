# calcha
One-pass mathematical equation parser written in the Hare Programming Language.

## Installation
### Prerequisite Software
Before you are able to install the Calcha compiler, you will need to install two other pieces of software:

1. [Install QBE Compiler Backend](https://c9x.me/compile/) -
More verbose installation instructions for QBE will come soon, but for now please follow the instructions in the repository from the link above after you have cloned the repository to your local system

2. [Install Hare Programming Language](https://harelang.org/documentation/install/index.html) -
Please note there is third-party support for MacOS, but this is considerably harder than spinning a quick VM

### Cloning Calcha Repository
Before building the Calcha compiler, you will need to clone the repository to your local system:
```sh
git clone --depth=1 git@github.com:NAU-OSS/calcha.git
cd calcha
```

### Install Calcha On Your System
Once you have obtained the above software, installing Calcha is as easy as the following command:
```sh
sudo make install
```

### Install Calcha Without Root Access
If you are installing to a system to which you do not have root permissions, then you can simply install Calcha for your user with the following command:
```sh
make install INSTALL_PREFIX=/path/to/install
```
Where `/path/to/install` is a directory to which you have read and write access; a typical choice for installation is in `~/.local`

If you set a different install path than the default (e.g. `/usr/local`), please remember to update your `PATH` environment variable with the following command:
```sh
export PATH="$PATH:/path/to/install"
```
This way you can use Calcha from anywhere in the filesystem

## Usage examples

## Status
Not implemented

## Contact
Email: ajh728@nau.edu

GitHub: @Asa-Henry
