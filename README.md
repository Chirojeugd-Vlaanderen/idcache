#be.chiro.civi.idcache

This extension provides functions to retrieve ID's of CiviCRM entities
based on their names. It uses CiviCRM's cache to reduce database access.

The idea is to use this in combination with 
[org.civicoop.configitems](https://github.com/CiviCooP/org.civicoop.configitems).

An example might make things clear:

    // retrieve the group id of the group with name mygroup.
    $myGroupId = CRM_IdCache_Cache_Generic::getId('Group', 'mygroup');
