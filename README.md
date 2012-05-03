kickstarter
===========

Kickstart file generator based on YAML formated meta data

Installation
------------

Install cheetah (http://www.cheetahtemplate.org/) templating system, PyYAML.

run make
sudo python setup.py install

Usage
-----

kickstarter -c <images.yaml> -r <repos.yaml>

Example:

    kickstarter  --configs configurations.yaml --repos repos.yaml 

This configuration.yaml file is an example only, for meego kickstart files,
consult the image-configurations package

Repo file
---------

This file contains a list of repositories to be used in the kickstart files

Configurations file
-------------------

This file has the definition of configurations. The Configurations inherit 
from platforms first then from the DEFAULT section. The image configurations
override the all other settings (in DEFAULT and platform sections).
