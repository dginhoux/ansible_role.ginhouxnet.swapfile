Ansible Role : dginhoux.swapfile
=========

This ansible role simply create a swapfile and enable it ; it can also disable and remove it.
There no way to expand an existing swapfile, it must be disabled and removed, before be recreated at the new size.


Requirements
------------

This role require a supported platform defined in `meta/main.yml`.
It will skip node with unsupported platform ; this behaviour can be bypassed by settings this variable `asserts_bypass=True`.


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
