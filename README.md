ginhouxnet.swapfile
=========

This ansible role simply create a swapfile and enable it ; it can also disable and remove it.
There no way to expand an existing swapfile, it must be disabled and removed, before be recreated at the new size.


Requirements
------------

This ansible role will only run on identified OS defined on meta/main.yml


Role Variables
--------------

It's just a simple list like : 

```
swap_file_path: /swapfile
swap_file_size_mb: '2048'

swap_file_state: present
```


Dependencies
------------




Example Playbook
----------------



License
-------

BSD


Author Information
------------------

Dany GINHOUX
