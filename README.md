This is a project template for ECE 5780, Embedded Systems.

# Installation
## Local Machine
Download and install Visual Studio Code.

https://code.visualstudio.com/

Some additional instructions for WSL on Windows.

https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode

Windows users will need to install PuTTY

https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

## Unix installation
Students are required to work in a Unix environment for this course.
If you wish, you may install Linux as your primary operating system, otherwise you will set up a virtual environment.
Mac OSX is a Unix variant, and can be used as the primary operating system..

### OSX
You will need to install brew.

https://brew.sh/

From there, install the package dependencies.
```
brew tap caskroom/cask
brew install cask gcc-arm-embedded
brew install openocd
brew install stlink
```


### WSL
The Windows Subsystem for Linux (WSL) allows installation of a Linux environment inside of Windows.

https://learn.microsoft.com/en-us/windows/wsl/install

### VirtualBox
VirtualBox creates a virtual machine, a full isolated computer environment with a separate operating system.

https://www.virtualbox.org/

### NoMachine
The CADE lab has all software needed already installed.
You will need to install NoMachine for USB forwarding.
We will not be using the GUI

https://www.nomachine.com/

https://www.nomachine.com/getting-started-with-nomachine

## Package installation
For Debian based systems (including Ubuntu and Mint), you will need to install the following packages.
```
apt-get install stlink-tools gcc-arm-none-eabi binutils-arm-none-eabi make git
```

# Development process
## Attach USB device
To work with your microcontroller in your environment, you will need to attach the USB device.

### WSL
https://learn.microsoft.com/en-us/windows/wsl/connect-usb

### VirtualBox
https://www.virtualbox.org/manual/topics/BasicConcepts.html#usb-support

### NoMachine

https://kb.nomachine.com/DT10K00060#4.3

# Drivers
This repository contains libraries copied from https://github.com/STMicroelectronics/STM32CubeF0 at commit 165396863a295fe41640f721f8b8ba276572e083.
License information for these libraries is located inside library directories.
