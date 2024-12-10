test-builds
===========

GitHub repository to test different Read the Docs builds scenarios.

----

Read the Docs configuration file used to build this docs:

.. literalinclude:: ../.readthedocs.yaml
   :language: yaml
   :linenos:

----

Sphinx configuration file used to build this docs (:doc:`see full file <conf>`),

.. literalinclude:: conf.py
   :language: python
   :end-before: ###########################################################################
   :linenos:

----

.. runblock:: pycon

   >>> # Build at
   >>> import datetime
   >>> datetime.datetime.utcnow()  # UTC


.. sphinx_blog documentation master file, created by
   sphinx-quickstart on Mon Dec  9 09:06:36 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

sphinx_blog documentation
=========================

Add your content using ``reStructuredText`` syntax. See the
`reStructuredText <https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html>`_
documentation for details.


.. toctree::
   :maxdepth: 2
   :caption: Contents:

   file1
   file2
   file3
   file4
   publishing_html_file
