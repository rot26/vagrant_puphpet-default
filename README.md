# Vagrant + PuPHPet (Development LAMP VM)

## Description

This is my default setup for developing most LAMP stack web applications.  It uses Vagrant, PuPHPet and Puppet.

## Project Setup

_How do I, as a developer, start working on the project?_ 

1. _What dependencies does it have (where are they expressed) and how do I install them?_
	1. [Vagrant](https://www.vagrantup.com/) (>=v1.6)
	- Please download the proper package for your operating system and architecture.  [https://www.vagrantup.com/downloads.html](https://www.vagrantup.com/downloads.html) 
2. _How can I see the project working before I change anything?_
	1. After installing run this in your command terminal
	```shell
	vagrant up
	```
	- A tutorial for vagrant is available on the [Vagrant website](https://docs.vagrantup.com/v2/getting-started/index.html).

## Testing

_How do I run the project's automated tests?_

There are currently no tests for the project.  Please feel free to contribute.

## Requirements

- A connection to the internet
- Git (obviously)
- Vagrant
- VirtualBox, VMware, Docker, Hyper-V, _OR_ a Custom VM Provider. ([Read More...](https://docs.vagrantup.com/v2/providers/index.html))

## Deploying

### _How to setup the deployment environment_

1. Clone this git repository
```shell
git clone git@github.com:rot26/vagrant_puphpet-default.git
```
2. After installing Vagrant from [https://www.vagrantup.com/downloads.html](https://www.vagrantup.com/downloads.html) Run the following command in your terminal
```shell
vagrant up
```
Everything else is included in the puppet and vagrant configuration files.

- _Required environment variables or credentials not included in git._
- _Monitoring services and logging._

### _How to deploy_

## Troubleshooting & Useful Tools

_Examples of common tasks_

### Logging into the vagrant machine

```shell
vagrant up
vagrant ssh
```

### Accessing the webbrowser

_Preferred Method: vagrant HostManager_

(requires permission to change host machine's _hosts_ file)

```http
http://vagrant.dev/	
```

_Alternatively access via ip address_

```http
http://192.168.42.10:80
```

OR

```http
http://localhost:8080/
```

## Contributing changes

### Pull Requests

Please submit your changes via Pull Requests

### Internal git workflow

I use [Atlassian's SourceTree workflow](https://www.atlassian.com/git/workflows#!workflow-gitflow) with the following branches:

- master = _master_
- develop = _develop_
- feature = _feature/_
- release = _release/_
- hotfix = _hotfix/_
- support = _support/_
- versiontag = 

[Read More... at (https://www.atlassian.com/git/workflows#!workflow-gitflow)](https://www.atlassian.com/git/workflows#!workflow-gitflow)

## License

GPLv2

