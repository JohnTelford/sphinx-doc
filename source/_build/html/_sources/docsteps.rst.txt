Doc Steps
=========

 **source directory**
      The directory which, including its subdirectories, contains all source
      files for one Sphinx project.

* Take a look at `Sphinx    <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#hyperlinks>`_ the home of sphinx-doc 

* Take a look at `Installing Sphinx <https://www.sphinx-doc.org/en/master/usage/installation.html>`_ 

*  `Quick reStructuredText <https://docutils.sourceforge.io/docs/user/rst/quickref.html#details>`_ has the  details of the markup may be found on the reStructuredText page

* Execute cli :file:`sphinx-quickstart` to create the source directory

* make the :file:`/docs` directory in the source directory 
    * it is the GitHub Pages interface
    * create an empty file :file:`.nojekyll`

* add some text to :file:`testing.rst`

* add :file:`testing.rst` to :file:`index.rst` toctree

* test ``make html``

* add to the :file:`/Makefile` :

    ::

        GitHub Pages
            github:
                @make html
                @cp -a ./build/html/* ./docs

* test ``make github``

Previewing Web Page
--------------------------

Open the `index.html` file in the source directory /Docs file 
