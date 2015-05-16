Syntax
------
**Items**

Items are highlighted.

*Italic*, **Strong**, ``Inline Literal``, `Interpreted`, 
Syntax_


**Code**

.. code:: py
  
   import os
   print 'ok'


Section
-------

**Create a Section title**

``<C-E>s1`` to ``<C-E>s6``

Use ``<C-E>s3`` to create a level 3 title

A Level 3 title

**View current document's sections**

``:RivHelpSection`` or ``<C-E>hs``


**Insert the Table of Contents**

``:RivCreateContent`` or ``<C-E>cc``


Block
-----

**Create a literal-block**

``:RivCreateLiteralBlock`` or ``<C-E>cb``


**Create a explicit-mark**

``:RivCreateExplicitMark`` or ``<C-E>cm``

- this is a list
- this is a list
- this is a list
1. heloo
#. heloo
#. heloo
#. heloo

definition
    defi list sdfssdf
    sdfsdf
    sdfdsf

:author:
    TOdsdfsf,
    David

::
 
    hello
    nihao
    print 'hello' 

Footer
======
some footer [1]_.

second footer [#]_
some footer [#]_

.. [1] first footer
.. [#] second footer
.. [#] second footer

Citation
========
this is a [CIT2001]_

.. [CIT2001] a citiation

Link
====
this is a link_

.. _link: http://www.sina.com.cn

this is a example_

.. _example: 
   This is a cross reference


**Create a link**

``:RivCreateLink`` or ``<C-E>ck``

**Navigate between links** 

``:RivLinkNext`` ``:RivLinkPrev``,
or ``<Tab>`` and ``<S-Tab>`` in Normal Mode 

Image
-----
for instance:
.. image:: images/ball1.gif 

The |biohazard| symbol must be used on containers used to dispose of medical
waste.
.. |biohazard| image:: biohazard.png 


Table
=====

**Create a Grid Table** 

``:RivTableCreate`` or ``<C-E>tc``

+--------+----------------+
| ddfsdf | hellokjkjojsdf |
+--------+----------------+
|        |                |
| sdfsdf |                |
| sdffds |                |
+--------+----------------+




Table will be auto formatted when you leave insert mode.

In Insert mode:

    +-----------------------------------------+
    | Press ``<Enter>`` to create a new line  |
    | sdfsdfsdf hello                         |
    |                                         |
    |                                         |
    | hello                                   |
    +-----------------------------------------+
    | Press ``<C-Enter>`` to create a new row |
    | sdf                                     |
    | sdf                                     |
    +-----------------------------------------+

Insert a ``|`` to create new columns.

    +---+----------------+--------+
    | A | sdfsdfsdfTable | sdfsdf |
    +---+----------------+--------+


Todo
====
Things Todos

**Create todo item and toggle state**

On List lines, Press ``:RivTodoToggle`` or ``<C-E>ee``,
You can also click the todo items to toggle it's state.

    A. [ ] Press ``<C-E>ee`` to toggle the todo state.

**Change Priorities**

``:RivTodoPrior`` or ``<C-E>ep``

    A. [ ] Press ``<C-E>ep`` to toggle the todo prior

Note
=======
A place to hold your diaries or notes.

**Create scratch of Today**

``:RivScratchCreate`` or ``<C-E>sc``

**View Scratch Index**

``:RivScratchView`` or ``<C-E>sv``


Project
-------
Put your documents in a project

**Open main project's index file**

``:RivProjectIndex`` or ``<C-E>ww`` to 

**Show project list**

``:RivProjectList`` or ``<C-E>wa``

File
----
Link files

**File link in vim**

File with specified extensions will be highlighted and linked.

    index.rst ~/Documents/ test.py
    [[test]]

It's not converted, so in vim only.

**File link in other format**

To make links working after converting. 
Riv provide two styles::

    Moinmoin style: [[riv]]

    Sphinx style: :doc:`riv`

by default the Moinmoin style are used, 
and the links of this style will be converted.

If you are using Sphinx style. 
You must convert it using Sphinx_ toolkit.


Publish
=======

docutils_ package required.

**Convert document to other format**

``:Riv2HtmlAndBrowse`` or ``<C-E>2hh`` will convert current file to html and browse.

``:Riv2Odt`` or ``<C-E>2oo`` will convert current file to odt.

If you are working in a project.

``:Riv2HtmlProject`` will convert current project to html.
``:RivProjectHtmlIndex`` will open index in browser.


Helper
------
Help manage the document.

**Section Helper** 

``:RivHelpSection`` or ``<C-E>hs``

**File Helper**  

``:RivHelpFile`` or ``<C-E>hf``

**Todo Helper** 

``:RivHelpTodo`` or ``<C-E>ht``

