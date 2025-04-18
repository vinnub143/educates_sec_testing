Version 3.3.0
=============

New Features
------------

* Added `local resolver update` cli command to reload Resolver container in 
  case there's a change in local ip assigned to the computer running educates
  local.

* It is now possible via the REST API of the training portal and lookup service,
  when requesting a workshop, to provide a webhook URL to which analytics events
  pertaining to just that workshop session should be delivered.
