
My Title
=========
Donec ullamcorper nulla non metus auctor fringilla. Nullam quis risus eget urna mollis ornare vel eu leo. Vestibulum id ligula porta felis euismod semper. Aenean lacinia bibendum nulla sed consectetur. Curabitur blandit tempus porttitor. Aenean lacinia bibendum nulla sed consectetur.


Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Sed posuere consectetur est at lobortis. Curabitur blandit tempus porttitor. Donec ullamcorper nulla non metus auctor fringilla. Maecenas faucibus mollis interdum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut 


Setting up the documentation sources


Sphinx comes with a script called :program:`sphinx-quickstart` that sets up a
source directory and creates a default :file:`conf.py` with the most useful
configuration values from a few questions it asks you. To use this, run:

.. code-block:: shell

Getting Started
===============

   -a            command-line option "a" 
   -b file       options can have arguments 
              and long descriptions 
   --long        options can be long also 
   --input=file   long options can also have 
              arguments 
  /V            DOS/VMS-style options too

A paragraph containing only two colons 
indicates that the following indented 
or quoted text is a literal block. 

:: 

  Whitespace, newlines, blank lines, and 
  all kinds of markup (like *this* or 
  \this) is preserved by literal blocks. 

  The paragraph containing only '::' 
  will be omitted from the result. 

The ``::`` may be tacked onto the very 
end of any paragraph. The ``::`` will be 
omitted if it is preceded by whitespace. 
The ``::`` will be converted to a single 
colon if preceded by text, like this:: 

  It's very convenient to use this form. 

Literal blocks end when text returns to 
the preceding paragraph's indentation. 
This means that something like this 
is possible:: 

      We start here 
    and continue here 
  and end here. 

Per-line quoting can also be used on 
unindented literal blocks:: 

> Useful for quotes from email and 
> for Haskell literate programming.

Sphinx is a *documentation generator* or a tool that translates a set of plain
text source files into various output formats, automatically producing
cross-references, indices, etc.  That is, if you have a directory containing a
bunch of :doc:`/usage/restructuredtext/index` or :doc:`/usage/markdown`
documents, Sphinx can generate a series of HTML files, a PDF file (via LaTeX),
man pages and much more.

Sphinx focuses on documentation, in particular handwritten documentation,
however, Sphinx can also be used to generate blogs, homepages and even books.
Much of Sphinx's power comes from the richness of its default plain-text markup
format, :doc:`reStructuredText </usage/restructuredtext/index>`, along with
it's :doc:`significant extensibility capabilities </development/index>`.

The goal of this document is to give you a quick taste of what Sphinx it is and
how you might use it. When you're done here, you can check out the
:doc:`installation guide </usage/installation>` followed by the intro to the
default markup format used by Sphinx, :doc:`reStucturedText
</usage/restructuredtext/index>`.

For a great "introduction" to writing docs in general -- the whys and hows, see
also `Write the docs`__, written by Eric Holscher.

.. __: http://www.writethedocs.org/guide/writing/beginners-guide-to-docs/


   $ sphinx-quickstart

Grid table:

+------------+------------+-----------+ 
| Header 1   | Header 2   | Header 3  | 
+============+============+===========+ 
| body row 1 | column 2   | column 3  | 
+------------+------------+-----------+ 
| body row 2 | Cells may span columns.| 
+------------+------------+-----------+ 
| body row 3 | Cells may  | - Cells   | 
+------------+ span rows. | - contain | 
| body row 4 |            | - blocks. | 
+------------+------------+-----------+

.. DANGER::
   Beware killer rabbits. Yea they are mean!

.. note:: This is a note admonition.
   This is the second line of the first paragraph.

   - The note contains all indented body elements
     following.
   - It includes this bullet list.

.. list-table:: Frozen Delights!
   :widths: 15 10 30
   :header-rows: 1

   * - Treat
     - Quantity
     - Description
   * - Albatross
     - 2.99
     - On a stick!
   * - Crunchy Frog
     - 1.49
     - If we took the bones out, it wouldn't be
       crunchy, now would it?
   * - Gannet Ripple
     - 1.99
     - On a stick!

     .. |date| date:: %b %d, %Y
.. |time| date:: %H:%M

Today's date is |date|.

This document was generated on |date| at |time|.
