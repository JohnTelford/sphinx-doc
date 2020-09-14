Doc Steps
------------

- Take a look at `Sphinx    <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#hyperlinks>`_. It is the home of sphinx-doc 

- `Quick reStructuredText <https://docutils.sourceforge.io/docs/user/rst/quickref.html#details>`_ has the  details of the markup may be found on the reStructuredText page

- `sphinx-quickstart`

- add test to testing.rst

- add test doc to /source: testing.rst

- add testing.rst to index.rst toctree

- make `/docs` directory 
    - this is the GitHub Pages interface
    - create an empty file `.nojekyll`

- `make html`

- add to the Makefile:

    ::

        GitHub Pages
            github:
                @make html
                @cp -a ./build/html/* ./docs

- next