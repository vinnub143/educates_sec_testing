Version 3.3.2
=============

Bugs Fixed
----------

* A reserved session which had existed for longer than the inactivity time,
  and which had just been allocated could be incorrectly seen as being orphaned
  and deleted, if the cleanup task ran in the small period of time between the
  reserved session being allocated and activated.
