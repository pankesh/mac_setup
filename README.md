# My Mac Setup   [![Build Status](https://travis-ci.org/mchidzik/mac_setup.svg?branch=master)](https://travis-ci.org/mchidzik/mac_setup)

The purpose is to aid the setup/configuration/update of my Mac OS setup. 

## First steps.
Install homebrew, see: http://brew.sh

Install homebrew cask, see https://caskroom.github.io/

````
brew tap caskroom/cask
````

## Install ansible

````
brew install ansible
````

## Running this playbook:
First update the vars/main.yml file with the software you want on your Mac. Then run the playbook.


````
ansible-playbook ./setup.yml -v
````

or alternatively
````
./setup.yml
````

----

## More setup needed:
- install java from Oracle
- install xcode, from the App Store
- docker for mac, see https://docs.docker.com/docker-for-mac/
- zsh
- dot files
- git command completion

## Brew commands to periodically run:

- brew update              # to update formulae and Homebrew
- brew outdated            # find out what's outdated
- brew upgrade             # upgrade everything
- brew upgrade <formula>   # upgrade only specific formula
- brew cleanup             # to cleanup old versions; Note: Homebrew does not uninstall old versions of a formula
- brew --cache             # where stuff gets downloaded

