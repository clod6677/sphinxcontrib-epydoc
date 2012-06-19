####################
sphinxcontrib-epydoc
####################

http://sphinxcontrib-epydoc.readthedocs.org

A Sphinx_ extension to cross-reference epydoc-generated documentation.

Installation
------------

This extension can be installed from the `Python Package Index`_::

   pip install sphinx-contrib.epydoc


Usage
-----

Add this extension to ``extensions`` and configure the cross-reference mapping::

   extensions = ['sphinxcontrib.epydoc']

   epydoc_mapping = {
      'http://paludis.exherbo.org/api/python/': [r'paludis(\.|$)'],
   }

Now you can reference identifiers from Paludis_ with the standard directives
from the Python domain::

   This is a cross-reference to :class:`paludis.PackageID`.

For more details refer to the documentation_, though there really isn't much
more.


.. _`Sphinx`: http://sphinx.pocoo.org/latest
.. _documentation: http://sphinxcontrib-epydoc.readthedocs.org
.. _python package index: http://pypi.python.org/pypi/sphinxcontrib-epydoc
.. _paludis: http://paludis.exherbo.org/api/python/index.html
