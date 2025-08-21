Version 3.3.3
=============

Features Changed
----------------

* The ``EDITOR`` environment variable is now set to ``/usr/bin/vim`` for
  terminal sessions as some tools can require the ``EDITOR`` environment
  variable be set.

Bugs Fixed
----------

* The custom resource definition for `Workshop` was missing the `path` property
  when defining `ingresses`.
