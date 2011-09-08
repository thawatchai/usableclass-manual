Introduction
------------

This repository contains the source for help.class.in.th.

To build the output documents, you need a mac with several tools as described below.

Set Up
-------

You must have these tools installed in your mac:

* Xcode
* MacPorts
* MacTeX
* Thai SIPA Fonts
* Thai TEPC Fonts

Run these commands to install Python 2.7

::

  sudo port -uv install python27
  sudo port select --set python python27

Run these commands to install Sphinx

::

  sudo port -uv install py27-sphinx
  sudo ln -s /opt/local/bin/sphinx-build-2.7 /opt/local/bin/sphinx-build
  
Run these commands to clone this repo

::

  cd ~/workspace
  git clone git@github.com:thawatchai/usableclass-manual.git
  cd usableclass-manual
  
Run these commands to build the targets

::

  make html
  make latex; make pdf