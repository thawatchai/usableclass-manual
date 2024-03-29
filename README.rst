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
* Kod

Add this line to your .bashrc.

::

  PATH=$PATH:~/bin:/usr/texbin

Run these commands to install Python 2.7.

::

  sudo port -uv install python27
  sudo port -uv install python_select
  sudo port select --set python python27

Run these commands to install Sphinx.

::

  sudo port -uv install py27-sphinx
  sudo ln -s /opt/local/bin/sphinx-build-2.7 /opt/local/bin/sphinx-build
  
Run these commands to clone this repository.

::

  cd ~/workspace
  git clone git@github.com:thawatchai/usableclass-manual.git
  cd usableclass-manual
  sh setup.sh
  
Run these commands to edit and build the targets.

::

  kod .
  make html
  make latex; make pdf

Screen Capturing
------------------

We capture screenshots using Skitch for partial shots and Screengrab! FireFox addon for whole-page shots. Skitch and Preview are used to resize and crop images.

License
--------

Copyright © 2011 Thawatchai Piyawat, Jantawan Piyawat, Nantita Noiwan

CC-BY-NC