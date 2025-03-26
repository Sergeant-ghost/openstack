DevStack is a set of scripts and utilities to quickly deploy an OpenStack cloud
from git source trees.

Goals
=====

* To quickly build dev OpenStack environments in a clean Ubuntu or RockyLinux
  environment
* To describe working configurations of OpenStack (which code branches
  work together?  what do config files look like for those branches?)
* To make it easier for developers to dive into OpenStack so that they can
  productively contribute without having to understand every part of the
  system at once
* To make it easy to prototype cross-project features
* To provide an environment for the OpenStack CI testing on every commit
  to the projects

Read more at https://docs.openstack.org/devstack/latest

IMPORTANT: Be sure to carefully read `stack.sh` and any other scripts you
execute before you run them, as they install software and will alter your
networking configuration.  We strongly recommend that you run `stack.sh`
in a clean and disposable vm when you are first getting started.



Customizing
===========

DevStack can be extensively configured via the configuration file
`local.conf`.  It is likely that you will need to provide and modify
this file if you want anything other than the most basic setup.  Start
by reading the `configuration guide
<https://docs.openstack.org/devstack/latest/configuration.html>`_
for details of the configuration file and the many available options.
