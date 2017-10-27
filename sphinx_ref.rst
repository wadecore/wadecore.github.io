Formatting for Sphinx
=====================

This text will not appear bold even without indentation because it is directly following the main header. This is used for the main description of all that is to follow.

Subsection about text
--------------------

This text will appear in bold unless you indent it. this operates as a form of header
    Indented paragraphs will appear as normal, unbolded text unless a markup has been applied

    You can also markup things such as *italics*, **bold face**, and ``code`` inline in paragraphs, but you can't nest those, start or end them with a space, so be careful.

dot dot markup type colon colon
-------------------------------

.. attention::
    indent the text so that it appears in the box

.. caution::
    indent the text so that it appears in the box

.. danger::
    indent the text so that it appears in the box

.. error::
    indent the text so that it appears in the box

.. hint::
    indent the text so that it appears in the box

.. important::
    indent the text so that it appears in the box

.. note::
    indent the text so that it appears in the box

.. tip::
    indent the text so that it appears in the box

.. warning::
    indent the text so that it appears in the box

.. admonition:: custom content label
    indent the text so that it appears in the box

Lists
-----

hey take a look at this bulleted list
* bulleted lists use your
* indentations to decide
  * what level the information
  * is on
* you can go back to the parent list
  * if you need to
    * or you can go
      * deeper
        * and deeper

how about this numbered list
1. you can make numbered lists
2. manually

or this one
#. or you can make them
#. automatically



Links, Images, Code Samples, Tables
-------------------------------------

Links
  so I can put this `link to robotgeek <http://www.robotgeek.com>`_ in the middle of a bunch of text, or wherever really it's simple.

  or if you want to reference a list of links, you can do that shit too, `check`_ `this`_ `shit`_ `out`_.

.. _check: http://www.trossenrobotics.com
.. _this: http://www.robotgeek.com
.. _shit: http://www.interbotix.com
.. _out: http://www.github.com

 maybe you want to |pop_link|.

.. |pop_link| raw:: html

   <a href="http://www.readthedocs.org" target="_blank">open a link in a new tab</a>


Images
  You're just gonna have to get a load of this:

  You can point directly at the image easy peasy
.. image:: http://i0.kym-cdn.com/photos/images/original/000/616/992/4d2.png
  :width: 500

Code Samples

  Apparently this doesn't work very well, but to show a whole block of code, you just put colon colon after this and indent the lines of the code one more level to follow::
    #define arsehouse 0;
    #define hamshack 1;

    setup()
    {
      arsehouse = LOW ;
      hamshack = HIGH ;
    }

    loop()
    {
      //some nonsense involving a hamshack and an arsehouse, I suppose;
    }

just drop back a level to return to your regularly scheduled text. maybe we should just link to the github for code like we usually do.

.. you can also comment out things so that the front end doesn't see them at all

..
  like, even whole paragraphs of text
  with multiple lines
  as long as you indented after the comment
  and return to unindented afterwards

there be comments hidden above this line


Tables
  You can just straight up draw the tables. There's a couple ways to do it.

  +------------------------+------------+----------+----------+
  | Header row, column 1   | Header 2   | Header 3 | Header 4 |
  | (header rows optional) |            |          |          |
  +========================+============+==========+==========+
  | body row 1, column 1   | column 2   | column 3 | column 4 |
  +------------------------+------------+----------+----------+
  | body row 2             | ...        | ...      |          |
  +------------------------+------------+----------+----------+

    and

  =====  =====  =======
  A      B      A and B
  =====  =====  =======
  False  False  False
  True   False  False
  False  True   False
  True   True   True
  =====  =====  =======

Raw Embeds
----------

Raw is a stop-gap for anything not natively supported by the sphinx compiler. We shouldn't use this super often but we're totally going to.

Embed file (put a broken embed file before embedding a page to prevent tree stacking)

.. raw:: html
   :file: inclusion.html

Embed Entire Page (GitHub Code)

.. raw:: html
   :url: https://raw.githubusercontent.com/wadecore/spriteDisplay/master/spriteDisplay.ino

Embed entire Page (Fusion360)

.. raw:: html
   :url: http://www.trossenrobotics.com/Shared/readthedocs/a360embed.html

Embed entire Page (SketchFab)

.. raw:: html
   :url: http://www.trossenrobotics.com/Shared/readthedocs/sketchfabembed.html

Embed entire Page (Youtube Video)

.. raw:: html
   :url: http://www.trossenrobotics.com/Shared/readthedocs/videoembed.html


