Version 3.3.3
=============

Features Changed
----------------

* The ``EDITOR`` environment variable is now set to ``/usr/bin/vim`` for
  terminal sessions as some tools can require the ``EDITOR`` environment
  variable be set.

* For reasons that have been forgotten, the ``XDG_CONFIG_HOME`` environment
  variable was being set to ``/tmp/.config``. Overriding this was problematic
  when some tools/scripts assumed standard location of ``~/.config``, but
  others honoured ``XDG_CONFIG_HOME``. No longer setting this environment
  variable. If a workshop has issues when standard location is used, it will
  need to override it as part of workshop.

Bugs Fixed
----------

* The custom resource definition for `Workshop` was missing the `path` property
  when defining `ingresses`.
