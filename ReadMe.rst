``EDITOR`` Helpers
==================

:Author: Ben Spaulding

This is a collection of helper scripts for using popular Mac text editors as
your terminal ``EDITOR``.

These are certainly not essential, as all of the editors helped here ship with a
powerful command-line utility. However, to properly use them for something like
editing a git commit message the editor must not fork, and must wait for you to
do your work, then return focus to the terminal. This is done by passing
switches and arguments to the utility. Unfortunately, some software — notably
``crontab`` — chokes on a multi-argument ``EDITOR``. The solution is to use a
wrapper script that calls the switches and arguments for you. That is just what
these helpers do.

Helpers are included for:

* BBEdit_
* TextWrangler_
* MacVim_

Notably absent is TextMate_, because no helper is necessary. See the details in
the `TextMate manual`_.

.. _BBEdit: http://www.barebones.com/products/bbedit/
.. _TextWrangler: http://www.barebones.com/products/textwrangler/
.. _MacVim: http://code.google.com/p/macvim/
.. _TextMate: http://macromates.com/
.. _TextMate manual: http://manual.macromates.com/en/using_textmate_from_terminal.html#the_general_editor_variable
