Version 3.3.1
=============

Bugs Fixed
----------

* When enabling `docker` for a workshop session, and the local registry mirror
  option was enabled, the latter was not actually working and no local caching
  within the cluster of pulled images was being performed. This previously
  worked but stopped working with Educates version 2.1.0, but this had not been
  noticed since it is a hidden caching mechanism and image pulls would still
  have worked.
