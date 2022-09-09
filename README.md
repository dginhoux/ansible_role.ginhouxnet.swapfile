Ansible Role : dginhoux.swapfile
=========

This ansible role simply create a swapfile and enable it ; it can also disable and remove it.
There no way to expand an existing swapfile, it must be disabled and removed, before be recreated at the new size.


Requirements
------------

This role is built to only run on platforms defined in `meta/main.yml`


Role Variables
--------------

```yaml
swap_file_path: /swapfile
swap_file_size_mb: '2048'

swap_file_state: present
```


Dependencies
------------

none


Example Playbook
----------------



License
-------

BSD


Author Information
------------------

https://github.com/dginhoux/
