.. this is master file, created by
   sphinx-quickstart on Tue May 27 11:24:59 2014.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Sphinx-doc as Notebook
==============================

This is the template for building your notebook using sphinx-doc.

Sphinx-doc was originally developed for automatic documenting your python code. However I found it being very useful for writing technical documents with the explicit and easy to remember syntax of restructuredText markup language. For several years I have been using sphinx for note-taking in my whole graduate student life. It has proven being very helpful to my research and life.

I probably can convince you by listing serveral of sphinx-doc's fantanstic stuff.

1. It is easy to install and use, as long as you have python installed on your computer. You could simple start a project without any customizations and it would be perfectly fine.
2. Sphinx-doc can produce multiple outputs of all kinds of file formats, including html, pdf, epub.
3. Math equations with numbering, figures, tables, references and citations, are all supported.
4. It's easily customized, including theming, extension developping.

There are many possible practices of sphinx-doc. My approach is to host source code on GitHub and allow readthedocs.org to automatically generate my html website for me. As for those private notes that you need to keep secret, aerobatic.com with passward protection is a great choice.

In this template, I will demonstrate the typography.


.. toctree::
   :maxdepth: 3
   :numbered:

   introduction/index.rst
   group-meeting/index.rst
