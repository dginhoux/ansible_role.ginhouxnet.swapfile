# ROLE dginhoux.swapfile



## DESCRIPTION

This ansible role create a swapfile and enable it ; it can also disable and remove it.<br />
There no way to expand an existing swapfile, it must be disabled and removed, before be recreated at the new size.




## REQUIREMENTS

#### SUPPORTED PLATFORMS

| Platform | Versions |
|----------|----------|
| Debian | all |
| EL | all |
| Fedora | all |
| Ubuntu | all |

#### ANSIBLE VERSION

Ansible >= 2.13

#### DEPENDENCIES

None.



## INSTALLATION

#### ANSIBLE GALAXY

```shell
ansible-galaxy install dginhoux.swapfile
```
#### GIT

```shell
git clone https://github.com/dginhoux/ansible_role.swapfile dginhoux.swapfile
```


## USAGE

#### EXAMPLE PLAYBOOK

```yaml
- hosts: all
  roles:
    - name: start role dginhoux.swapfile
      ansible.builtin.include_role:
        name: dginhoux.swapfile
```


## VARIABLES

#### DEFAULT VARIABLES

Defaults variables defined in `defaults/main.yml` : 

```yaml
swap_file_path: /swapfile
swap_file_size_mb: '2048'

swap_file_state: present
```

#### DEFAULT OS SPECIFIC VARIABLES

Those variables files are located in `vars/*.yml` are used to handle OS differences.<br />
One of theses is loaded dynamically during role runtime using the `include_vars` module and set OS specifics variable's.

`NOT USED BY THIS ROLE`



## AUTHOR

Dany GINHOUX - https://github.com/dginhoux



## LICENSE

MIT
