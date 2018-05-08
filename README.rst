*****************************************
Can packaging improve Django deployments?
*****************************************

How can packaging Django projects make deployments easier, faster and more reliable?

Deployments of Django projects can be a challenging task. Beside the Python source code itself you usually have to handle a lot of other stuff:

* Installing Python dependencies
* Shipping JavaScript code and installing it's dependencies
* Compiling SCSS to CSS
* Collecting static files
* Building documentation
* Compiling translations
* …

And of course you want a deployment approach that is independent of a specific hosting solution.

Also you have to think about the scalability of your deployment when the number of servers you operate increases.

This usually means that `git pull` is not the best way to deal with these tasks.

So I will discuss different ways to package your Django project like

* Wheels
* JavaScript packages
* Operating system packages
* Containers

Some of these concepts will hopefully help you to make your deployment process easier, faster and more reliable.

Requirements
============

You have to install the following requirements to build and serve the
presentation:

- `npm <https://www.npmjs.com/>`_
- `Python 3.4 <https://www.python.org/>`_ or newer

Installing and linking the dependencies
=======================================

You can install and link all required resources by running

::

    $ make link

Running the presentation
========================

You can serve the slides by running

::

    $ make serve

Controlling the presentation
============================

- Use the *SPACE BAR* to move to the next slide.
- Use the *arrow keys* to move around.
- Use the *F* key to enter full screen mode. Press the *ESC* key to leave it again.
- Use the *S* key to open the moderator monitor containing the notes.
- Use the *B* key to make the screen dark. Push the same key to brighten the screen again.
- Use the *ESC* key to enter the bird's-eye view showing all slides. Then use the *arrow keys* to move around.

Showing all tasks in the ``Makefile``
=====================================

You can show all tasks in the ``Makefile`` by running

::

    $ make

License
=======

This work is licensed under a
`Creative Commons Attribution 4.0 International License <http://creativecommons.org/licenses/by/4.0/>`_.
