system_groups
=============

[![Ansible Galaxy][galaxy_image]][galaxy_link]
[![Build Status][travis_image]][travis_link]
[![Latest Tag][tag_image]][tag_link]

An [Ansible](https://www.ansible.com/) role to manage system groups.

Group `root` can't be managed using this role for security reasons.

Requirements
------------

None.

Role Variables
--------------

```yaml
# list of system groups
system_groups__list: []
## group name
#  - name: string
## OPTIONAL: if set to true, group is removed from host
#    disabled: bool
## OPTIONAL: group id
#    gid: int
## OPTIONAL: system group flag
#    system: bool
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - role: "tomashavlas.system_groups"
      system_groups__list:
          - name: "usergrp"
            gid: 1564
          - name: "systemgrp"
            system: true
          - name: "disabledgrp"
            disabled: true
```

For more examples see [test cases](https://github.com/tomashavlas/ansible-role-system_groups/tree/master/tests).

License
-------

BSD

Author Information
------------------

Created by [Tomáš Havlas](https://github.com/tomashavlas) in 2016.

[galaxy_image]: https://img.shields.io/badge/galaxy-tomashavlas.system__groups-blue.svg?style=flat
[galaxy_link]: https://galaxy.ansible.com/tomashavlas/system_groups/
[tag_image]: https://img.shields.io/github/tag/tomashavlas/ansible-role-system_groups.svg
[tag_link]: https://github.com/tomashavlas/ansible-role-system_groups/tags
[travis_image]: https://travis-ci.org/tomashavlas/ansible-role-system_groups.svg?branch=master
[travis_link]: https://travis-ci.org/tomashavlas/ansible-role-system_groups/
