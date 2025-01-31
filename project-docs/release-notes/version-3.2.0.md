Version 3.2.0
=============

New Features
------------

* Added `--hostname` option for overridding generated hostname when creating a
  portal using the `educates create-portal` command. If only a single host name
  is given, the existing cluster ingress domain will still be added. If a fully
  qualified domain name is given it will be used as is.
