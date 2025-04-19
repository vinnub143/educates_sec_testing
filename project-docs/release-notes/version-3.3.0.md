Version 3.3.0
=============

New Features
------------

* Added `local resolver update` CLI command to reload Resolver container in 
  case there's a change in local ip assigned to the computer running educates
  local.

* It is now possible via the REST API of the training portal and lookup service,
  when requesting a workshop, to provide a webhook URL to which analytics events
  pertaining to just that workshop session should be delivered.

Bugs Fixed
----------

* When the lookup service was being deployed and an insecure ingress was being
  used to access it, clients were being incorrectly redirected to a secure
  ingress, resulted in an error since only insecure access was being expected.

* When deploying a workshop to a local docker environment using the `educates`
  CLI it would fail if the local registry hadn't previously been deployed as it
  was trying to map the docker network for the registry when not required.
