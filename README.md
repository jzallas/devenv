# devenv
## Overview
This is a local development environment that I use for the purposes of building and running applications on different operating systems. For now, this will just be a convenient way to spin up an docker enabled environment on the off-chance that an application needs to be run on an operating system where installing native docker isn't trivial.

## What's included?
1. Ubuntu 14.04.5 LTS
1. Docker CE

## Requirements
This may work on other versions, but these are the specific versions I am using and have tested
1. Install Vagrant v.1.9.7
1. Virtualbox v.5.1.24

## Usage
1. You should install the vb-guest plugin to ensure that shared folders work properly:
`vagrant plugin install vagrant-vbguest`
1. `vagrant up`
1. Optional: to validate that everything is working:
```
vagrant ssh
sudo docker run hello-world
```

## TODO
At some point I will include a description on how to install and run docker images using this environment.
