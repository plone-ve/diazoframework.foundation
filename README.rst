=========================
diazoframework.foundation
=========================


Introduction
============

``diazoframework.foundation`` package provides the diazo framework implementation 
of the `Zurb Foundation CSS framework`_ using the **theming** and **packaging** 
features available for create Diazo_ theme using `plone.app.theming`_. 

They are useful for creating themes based on `Zurb Foundation CSS framework`_. 
A Diazo framework should provide the framework resources and diazo rules to reuse 
and add to in a Diazo theme.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*will be installed as a dependency of this package*)


Features
========

- Provides the *Zurb Foundation CSS framework* resources.
- Included Diazo rules for the **head** that contains ``base`` CSS styles.
- Included Diazo rules for the **body** that contains ``columns``, ``content``, ``footer``, 
  ``grid``, ``header``, ``lead`` and ``portlets`` CSS styles.


Installation
============


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``diazoframework.foundation`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        diazoframework.foundation


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'diazoframework.foundation',
    ],


Resources
=========

The resources of this framework can be reached through 
``/++framework++foundation`` and there are placed at 
``diazoframework.foundation/diazoframework/foundation/framework/`` 
directory with following resources files:


::

    _ css
    _ examples
    _ js
    _ rules
      _ body
        _ columns.xml
        _ content.xml
        _ footer.xml
        _ grid.xml
        _ header.xml
        _ lead.xml
        _ portlets.xml
      _ head
        _ base.xml
    _ humans.txt
    _ index.html
    _ preview.png
    _ robots.txt


Current themes
==============

The `diazoframework.foundation <https://github.com/TH-code/diazoframework.foundation>`_ package have the following themes:

- `diazotheme.foundation <https://github.com/TH-code/diazotheme.foundation>`_.


For more frameworks see: `diazoframework.plone <https://github.com/TH-code/diazoframework.plone#current-frameworks>`_


Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.foundation/issues
- Source Code: https://github.com/TH-code/diazoframework.foundation


License
=======

The project is licensed under the GPLv2.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/TH-code/diazoframework.foundation/contributors


.. _`Zurb Foundation CSS framework`: http://foundation.zurb.com/
.. _`diazoframework.foundation`: https://github.com/TH-code/diazoframework.foundation
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
