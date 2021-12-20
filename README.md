ansible-role-packages
=========

Install and remove packages.

Requirements
------------

RHEL7 or above

Role Variables
--------------

* `packages_install` - list of packages to install
* `packages_install_extra` - list of extra packages to install
* `packages_remove` - list of packages to remove
* `packages_remove_extra` - list of extra packages to remove

Dependencies
------------

Collections:

* `ansible.builtin`

Example Playbook
----------------

```
- hosts: myhosts
  vars:
    packages_install:
      - vim
    packages_remove:
      - nano
  roles:
    - ansible-role-packages
```

License
-------

GPLv3

Author Information
------------------

Vladimir Vasilev (@vladi-k)
