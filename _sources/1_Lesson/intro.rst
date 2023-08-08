=====================
This Is A New Course
=====================

SECTION 1: Introduction
:::::::::::::::::::::::

Congratulations!   If you can see this file you have probably successfully run the ``petljadoc init-course`` command.  

If you are looking at this as a source file you should now run ``petljadoc preview``  to generate html files and preview 
them in your browser.

This is just a sample of what you can do.  The index.yaml file is the table of contents for your entire project.



Section 2: Links
::::::::::::::::

Runestone uses the ``restructuredText`` (rst) markup language.  We chose this over markdown largely because rst is extensible.  Nearly all of the basic markup tasks are already handled by restructuredText.  You should check out the docs for the basics of restructuredText (link below). Our extensions are all for the interactive elements.  One key hint about restructuredText:  Its like **Python** -- *indentation matters!*

* Section `restructuredText <https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html>`_ from Sphinx Docs 
* `Runestone Author’s Guide <https://runestone.academy/runestone/static/authorguide/index.html>`_
* `PetljaDoc README <https://github.com/Petlja/PetljaDoc/blob/master/README.md>`_ 
* An Overview of Runestone Interactive `source <https://github.com/RunestoneInteractive/overview>`_ and 
  `published book <https://runestone.academy/runestone/static/overview/overview.html>`_
* A PetljaDoc project Textual Programming in Python `source code <https://github.com/Petlja/TxtProgInPythonEng/>`_ and 
  `public preview <https://petlja.github.io/TxtProgInPythonEng/>`_


SECTION 3: Sample Directives
::::::::::::::::::::::::::::::::::::::

ActiveCode
----------

.. activecode:: codeexample1
   :coach:
   :caption: This is a caption

   print("My first program adds a list of numbers")
   myList = [2, 4, 6, 8, 10]
   total = 0
   for num in myList:
       total = total + num
   print(total)


Now feel free to modify this file to start creating your own interactive page.
