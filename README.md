# Development Env and Vagrant 101


#### What is a Enviroment

Is a location where code runs and data lives

#### Dev Enviroment

The Developer Environment is where the developers write code, this will likely be on an individual's local machine.

#### 4 pillars of Devops

- Ease of use
	- Easy to use
	- If slow or buggy the developer will rebel

- Flexibility
	- Keep up with technology
	- Easy to change

- Robustness
	- 

- Cost


#### DevOps problems and solutions

Problem - "It works on my machine"
Standerdise the enviroments such as installing the latest version of PyCharm



## Vagrant & Virtual Box

### Virtual Box

VirtualBox is a general-purpose virtualization tool hardware, targeted at server, desktop, and embedded use, that allows users and administrators to easily run multiple guest operating systems on a single host

### Vagrant

Vagrant is a tool for building and managing virtual machine environments in a single workflow. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases production parity, and makes the "works on my machine" excuse a relic of the past.




### Package Manager


#### What is a package manager?

A package manager or package-management system is a collection of software tools that automates the process of installing, upgrading, configuring, and removing computer programs for a computer's operating system in a consistent manner.

#### What is python's package manager?

Pip, comes built in with python

#### What about other languages?

JavaScript - package.json


#### What are package managers for Windows and Mac?

Mac - Homebrew - software package management system that simplifies the installation of software on Apple's macOS operating system and Linux

Windows - Package Manager for Windows - Package Manager is the application installed on each machine to manage the installation and removal of the software contained in packages. Package Manager is configured to use one or more repositories as sources for packages.

#### What is the package manager for Ubuntu?

apt command (Advanced Packaging Too) - performing such functions as installation of new software packages, upgrade of existing software packages, updating of the package list index, and even upgrading the entire Ubuntu system.


#### NGINX

NGINX is a web server that can be used for web serving and also as a reverse proxy.




1. config.vm.box | This is our Operating System! We will be using ubuntu/xenial64 bit
2. config.vm.provider | This is VirtualBox
3. config.vm.network | How your host computer sees your box
4. config.vm.synced_folder | How you access files from your computer
5. config.vm.provision | What do we want to run as a provision for shell commands. What dependencies are needed? Node js? nginx?
If we dont use provisions, Vagrant will just run a blank ubuntu server

 

### Commands

 

1. vagrant init | Initiates Vagrant 
2. vagrant up | Activates Vagrant file and runs Virtual machine
3. vagrant suspends | Saves the virtual machine and suspend it / make it offline
4. vagrant resume | Resumes the virtual machine
5. vagrant destroy | Destroys the virtual machine
6. vagrant ssh | Makes us go inside of our virtual box. We can run | sudo apt-get update, 
sudo apt-get install nginx



