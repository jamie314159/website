Review
======

Today's Goals
-------------

* Working VM
* Run Systemview app
* Connect to Systemview from browser in host
* Understand what's happening

How to set up a VM
==================

Enable VirtualBox (VT extensions)
---------------------------------

Install `VirtualBox <https://www.virtualbox.org/wiki/Downloads>`_

Install `Vagrant <http://www.vagrantup.com/>`_

Linux
-----

.. code-block:: shell

    # clone
    git clone https://github.com/DevOpsBootcamp/devopsbootcamp-vagrant.git

    # start up
    cd devopsbootcamp-vagrant
    vagrant up

    # access vm
    vagrant ssh

IRC
===

* Use the `LUG guide <http://lug.oregonstate.edu/blog/irc/>`_ 
* #devopsbootcamp on irc.freenode.net
* Also join the `Mailing List
 <http://lists.osuosl.org/mailman/listinfo/devops-bootcamp>`_

GitHub Account
==============

SSH keys
--------

``ssh-keygen -t rsa``

Your public key is in ~/.ssh/id_rsa.pub by default. 

GitHub -> Account Settings (icon in upper right) -> SSH keys -> Add SSH key

Joining the organization
------------------------

* Ping edunham in the IRC channel to add you


Installing the Web App
======================

Prerequisite tools
------------------

On host machine, in devopsbootcamp-vagrant directory: 

.. code-block:: bash

    git pull
    vagrant up
    vagrant ssh


The Magic Script
----------------

Now that you're in the guest machine: 

.. code-block:: bash

    git@github.com:DevOpsBootcamp/catch-up.git

    cd catch-up
    ./catch-up.sh

Branches
--------

* Start one with ``git checkout -b branchname``
* Which are you on? ``git branch``
* Switch with ``git checkout branchname``

Connecting to the App
=====================

In the guest machine, with virtualenv activated, ``python systemview.py``

Point the browser of your host machine at 127.0.0.1:5050

If changes in the app don't show up in your browser, use f5 to hard refresh

Where am I?
===========

In virtual machine?
-------------------

* Did you ``vagrant ssh``?

In a repo?
----------

* ``git status``

On a branch?
------------

.. code-block:: bash

    # Show current branch
    $ git branch 

    # create new branch, called branchname
    $ git checkout -b branchname
