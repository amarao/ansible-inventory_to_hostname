Role Name
=========

Set up hostname to 'inventory_name_short'. Useful when you have your servers defined in ~.ssh/config, f.e.:

cat ~/.ssh/config

    Host lab2
        HostName 192.168.100.102
    Host lab3
        HostName 192.168.100.103
    ... etc


And you want to set up hostname for all you 'lab' hosts without binding it to any IP in ansible inventory.


Requirements
------------

None

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

    - hosts: lab*
      roles:
         - { inventory_to_hostname }

License
-------

BSD

Author Information
------------------

(c) George Shuklin, 2015
