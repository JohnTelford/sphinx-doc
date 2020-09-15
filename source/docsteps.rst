Doc Steps
=========


 Updated: |today|

**source directory**
    The directory which, including its subdirectories, contains all source
    files for one Sphinx project.

* Execute  the command ``<source directory>``:file:`sphinx-quickstart`  to create the source directory

* Take a look at `Sphinx    <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#hyperlinks>`_ home page

* Take a look at `Installing Sphinx <https://www.sphinx-doc.org/en/master/usage/installation.html>`_ 

*  `Quick reStructuredText <https://docutils.sourceforge.io/docs/user/rst/quickref.html#details>`_  has the  details of  ``reStructuredText`` markup 

* Make the  ``<source directory>``:file:`/docs` directory in the source directory 
    * It is the GitHub Pages interface
    * Create an empty file ``<source directory>``:file:`/docs`:file:`.nojekyll`

* Add some text to ``<source directory>``:file:`/testing.rst`

* Add :file:`testing.rst` to :file:`index.rst` toctree

* Test ``<source directory>````make html``

* Add this to the end of the ``<source directory>``:file:`/Makefile`

    # GitHub Pages
        github:
            @make html
            @cp -a ./build/html/* ./docs

* Test ``<source directory>/make github`` from the source directory

Previewing Web Page
--------------------------

Open the :file:`index.html` file in the source directory /Docs directory with a browser

====================  ==========  ==========
Header row, column 1  Header 2    Header 3
====================  ==========  ==========
body row 1, column 1  column 2    column 3
body row 2            Cells may span columns
====================  ======================