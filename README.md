# fuge-dev-environment

__CURRENTLY BEING SETUP! DON'T USE IF YOU SEE THIS MESSAGE__

An environment setup for building microservices with Fuge and SenecaJS. Uses Vagrant, Ansible and Docker.

Will install:

* Ubuntu (hashicorp/precise64 package)
* Git
* Curl
* Anisble
* Docker
* NodeJS 4.17
* Fuge NPM module
* Seneca NPM module 

## Requirements

[Vagrant](https://vagrantup.com) should be installed on your machine.

Vagrant in turn requires a VM provider to be installed, e.g. [VirtualBox](https://www.virtualbox.org/)

## Run

```vagrant up```

It'll take a while the first time unless you have the Vagrant box hashicorp/precise64 already setup.

## Starting and Stopping

### Start
```vagrant up``` (It'll take quite a while the first time)

### Stop
```vagrant halt```

### Reload
In case configuration has been changed
```vagrant reload```

## Shell Access

```vagrant ssh```

## Adding Code

Coming

## Destroying
If you want to completely clean up this virtual environment
```vagrant destroy -f```
