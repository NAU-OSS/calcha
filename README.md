# calcha
One-pass mathematical equation parser written in the Hare Programming Language.

Calcha is intended for computational hobbyist, professional, and researchers with an interest in accelerating mathematical processes using high performance hardware. Instead of using a general purpose programming language such as C, Python, etc., Calcha will take raw mathematical equations (written in reverse polish notation) and will do the work of translating the equations for the computer.

The advantage of Calcha is by passing the slowdown incurred by using languages such Python, and removes the need to possess any other knowledge about the computer to investigate mathematical inquery. On the other hand, Calcha is highly extensible, by allowing implementation of new code to carry out a mathematical process. Thus, the user is able to take full advantage of new hardware or to optimize existing processes to speedup a mathematical process.

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

## Usage Examples
### Basics
At the very basic, Calcha can be a calculator. Simply write a script - let's call this one `add.calcha`:
```c
5 4 +
```
Then, call the compiler and pass `add.calcha` to be compiled:
```sh
./ccalcha add.calcha
```
By default, `ccalcah` will run the resulting binary and provide you with the answer to the mathematical equation:
```sh
9
```

### Defining New Functions

### Optimizing Mathematical Processes

### Taking Advantage of New Hardware

## Status
This project is not implemented! Here is an outline of our following goals:
1. Implement basic mathematical operations (e.g. addition, subtraction, multiplication, division)
2. Allow for defining and using custom functions
3. Allow overriding of mathematical implementations
4. Allow for using specialized hardware

## Contact
Email: ajh728@nau.edu

GitHub: @Asa-Henry
