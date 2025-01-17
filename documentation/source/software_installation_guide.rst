Sofware Installation
====================

Installing the end-to-end system is a quite simple procedure, just performs the following steps .

Prerequisites
-------------

The system has been written using `python2.7 <https://www.python.org/download/releases/2.7/>`_. Hence be sure you have this language supported on your machine.
You will also an enough updated version of the following python libraries:

* `Numpy <http://www.numpy.org>`_, version 1.11.2 or higher.
* `Pandas <https://pandas.pydata.org>`_, version 0.20.3 or higher.
* `Scikit-learn <http://scikit-learn.org/stable/>`_ , version 0.18.1 or higher.

If you are familiar with packet management softwares like `macport <https://guide.macports.org/>`_, `homebrew <https://brew.sh/>`_, `apt <https://help.ubuntu.com/lts/serverguide/apt.html/>`_ or others, these will be a fairly easy task. Otherwise you can also install `anaconda <https://anaconda.org/>`_.
If you decide to adopt the latter, then be sure that also the :code:`accelerat` package is installed: once you have managed to install anaconda this can be easily achieved by typing

.. code-block:: console

   $ conda update conda
   $ conda install accelerate

Get the code
------------

Create a project folder, like

.. code-block:: console

   $ mkdir ${HOME}/Project_directory

in such folder, checkout a working copy of the code repository by tiping

.. code-block:: console

   $ git clone https://github.com/Fracappo87/XBTs_classification

then add the following line to your :code:`.bashrc` file

.. code-block:: shell

   export PYTHONPATH=$PYTHONPATH:$HOME/Project_directory/XBTs_classification

Run the code
------------

Before starting to use the system, move into the code directory and run all the tests:

.. code-block:: console

   $ cd $HOME/Project_directory/XBTs_classification
   $ python2.7 -m unittest discover

it will take less then one minute. If all the tests passed successfully you should see something like

.. code-block:: console

   $ cd $HOME/Project_directory/XBTs_classification
   $ python2.7 -m unittest discover
   ......................
   --------------------------------
   Ran XX tests in YYs

   OK

then you will be ready to use the **XBTs_classification** end-to-end system!
