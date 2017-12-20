.. _ch-intro:

************
Why Sphinx
************

.. role:: strike
   :class: strike

Writing notes? You probably are using LaTeX. LaTeX's good, no doubt. But, what if I need multiple output format out of one source? So they say, USE PANDOC.

You know pandoc. It's fast, easy to use. But I want to generate everything with one command.

"Check out the `Sphinx <http://www.sphinx-doc.org/>`_ project!"

Alright it's not made for writing notes or thesis. But J Terrace did write `a customized version (called sphinxtr) <https://github.com/jterrace/sphinxtr>`_ with everything you need for a thesis project, out of the box. However, the HTML theme is a little bit technical.

So I added bootstrap theme to sphinxtr. Checkout the `source <https://github.com/emptymalei/sphinx-notebook>`_.




.. admonition:: This is a Fork
   :class: warning

   This is a fork of `sphinxtr <https://github.com/jterrace/sphinxtr>`_. Almost everything is from there. I only added `bootstrap theme <https://ryan-roemer.github.io/sphinx-bootstrap-theme/>`_ and did a few adjustments.

   Many thanks to the maintainers of these projects.




Installation and Usage
========================



Basically just install everything in the ``requirements.txt``::

    pip install -r requirements.txt

Except that ``python-setuptools``, ``python-virtualenv``, ``texlive-full`` are to be installed first if you haven't.

| The following part is GRABBED from `installation guide for sphinxtr <https://github.com/jterrace/sphinxtr>`_.

#. `Install Sphinx <http://www.sphinx-doc.org/en/stable/tutorial.html#install-sphinx>`_, which in turn requires ``Python``. (I believe everyone installed python.)
#. `Setuptools <https://pypi.python.org/pypi/setuptools/1.1.6#installation-instructions>`_  (look for the most up to date version)
#. `Virtualenv <http://www.virtualenv.org/en/latest/#installation>`_
#. `Tex Live <http://www.tug.org/texlive/quickinstall.html>`_

Now create a virtualenv. This will help you to separate the requirements from
this project from other Python projects you might have::

    virtualenv venv
    source ./venv/bin/activate

.. note::

    You can get out of the virtualenv by either closing the terminal or by
    calling ``deactivate``.

Then install the required Python packages::

    pip install -r requirements.txt



To build the output with one line command, you need ``make``. The following targets are supported:

html
  Builds HTML format, separated into sections
singlehtml
  Builds HTML format on a single page
text
  Builds text files, separated into sections
singletext
  Builds a single text file
latexpdf
  Builds into latex source files and then compiles into a PDF. Requires latex.
