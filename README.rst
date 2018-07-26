=========================
diazoframework.foundation
=========================


Introduction
============

``diazoframework.foundation`` package provides the diazo framework implementation of the 
`Zurb Foundation CSS framework`_ using the **theming** and **packaging** features available in the 
`diazoframework.plone`_ core package for create `Diazo`_ theme using `plone.app.theming`_.

They are useful for creating themes based on `Zurb Foundation CSS framework`_. For documentation 
on the framework itself, check the website.

A Diazo framework should provide the framework resources and diazo rules to reuse 
and add to in a Diazo theme.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*You will need enable it via "Add-ons" control 
  panel to use this package*)
- The ``diazoframework.plone`` package (*You will need enable it via "buildout" 
  configuration to use this package*)


Features
========

- Provides the *Zurb Foundation CSS framework* v4.2.2 resources.
- Included Diazo rules for the **head** that contains ``base`` CSS styles.
- Included Diazo rules for the **body** that contains ``columns``, ``content``, ``footer``, 
  ``grid``, ``header``, ``lead`` and ``portlets`` CSS styles.


Installation
============

This add-on can be installed has any other add-ons. It's doesn't have any profile, so 
just add it to your Zope instance, for doing that please the follow steps: 


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
      _ foundation.css
      _ foundation.min.css
      _ normalize.css
    _ examples
      _ banded.html
      _ banner-home.html
      _ blog.html
      _ contact.html
      _ feed.html
      _ grid.html
      _ marketing.html
      _ orbit-home.html
      _ reality.html
      _ sidebar.html
      _ so-boxy.html
      _ store.html
      _ workspace.html
    _ humans.txt
    _ index.html
    _ js
      _ foundation
        _ foundation.alerts.js
        _ foundation.clearing.js
        _ foundation.cookie.js
        _ foundation.dropdown.js
        _ foundation.forms.js
        _ foundation.interchange.js
        _ foundation.joyride.js
        _ foundation.js
        _ foundation.magellan.js
        _ foundation.orbit.js
        _ foundation.placeholder.js
        _ foundation.reveal.js
        _ foundation.section.js
        _ foundation.tooltips.js
        _ foundation.topbar.js
      _ foundation.min.js
      _ vendor
        _ custom.modernizr.js
        _ jquery.js
        _ zepto.js
    _ preview.png
    _ robots.txt
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


Current themes
==============

The `diazoframework.foundation`_ package have the following themes:

`diazotheme.foundation`_
    which contains themes that can both be used as starters for your 
    own *Zurb Foundation CSS* based theme.


For more frameworks see: the `diazoframework.plone`_ package.


Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.foundation/issues
- Source Code: https://github.com/TH-code/diazoframework.foundation


License
=======

The project is licensed under the GPLv2.

The *Zurb Foundation CSS framework* is licensed under the MIT license.

The *normalize.css* is licensed under the MIT license.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/TH-code/diazoframework.foundation/contributors


.. _`Zurb Foundation CSS framework`: http://foundation.zurb.com/
.. _`diazoframework.plone`: https://github.com/collective/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`diazoframework.foundation`: https://github.com/TH-code/diazoframework.foundation
.. _`diazotheme.foundation`: https://github.com/TH-code/diazotheme.foundation
