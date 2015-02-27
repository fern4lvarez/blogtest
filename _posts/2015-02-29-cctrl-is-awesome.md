---
layout: post
title:  "Hello world"
date:   2015-02-29 14:21:33
---

`cctrl` is a set of command line utilities to help you create and manage applications
and users hosted on platforms compatible with [cloudControl](https://www.cloudcontrol.com).


Dependencies
------------

 * python 2.6.x or 2.7.x
 * python-setuptools
 * pip


Installation
------------
To install `cctrl`:

* Via pip (non-windows compatible)

    `$ (sudo) pip install cctrl`

* Via setup.py

    `$ (sudo) python setup.py install`


    Dependencies should be automatically fetched by `easy_install`.

* Via executable (windows only)

    https://www.cloudcontrol.com/download/win


To upgrade `cctrl` (non-windows compatible):

    $ (sudo) pip install cctrl --upgrade


To check successful installation of `cctrl`:

    $ cctrlapp -v
    cctrlapp 1.x.x using pycclib 1.x.x


Configuration
-------------

If you don't have an account yet, you can create it with this command:

    $ cctrluser create

Once you're done with installation and already have an account, you just
need to run one more command to get your setup ready:

    $ cctrluser setup

This command will save your email and the SSH public key you will use
to authenticate and to push with. See `cctrluser setup -h` for further
setup information.

Usage
-----

See `cctrlapp -h` to learn about its usage and available commands.


Vagrant Support
---------------

This project includes Vagrant support, so you can start an Ubuntu virtual machine
with your local `cctrl` version installed and ready to use. It might be also useful
for Windows users, so they can have a more Unix-like experience.