Version 3.2.1
=============

New Features
------------

* Added `uv`, a Python package and project manager, to the workshop base image.


Features Changed
----------------

* Updated `go` version for the CLI to 1.23.7 and other dependencies such as 
  kind, that now creates a Kubernetes 1.32.2 cluster. Minimal Docker Desktop 
  version that can be used has also been bumped to 4.34 released by end of 
  August 2024.

Bugs Fixed
----------

* Fixed generation of resolved images via kbld, so that descriptors and 
  configuration now has the sha256 resolved version of the images. This fixes
  the ability to create disconnected installs.

* Secrets were not being blocked from being injected by the Carvel
  `secretgen-controller` operator into namespaces created from
  `environment.objects`, `session.objects` and `request.objects` via the
  operators wildcard injection mechanism. These were being blocked for the
  session namespace and namespaces listed as secondary namespaces for sessions,
  but not namespaces manually included in `objects`. These are blocked due to
  the extreme risk from wildcard injection into any namespace since workshop
  session users can be untrusted users.
