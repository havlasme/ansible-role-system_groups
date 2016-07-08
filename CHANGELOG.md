Changelog
=========

Unreleased
----------

*Released: Unreleased*

- Added user prefix to Ansible roles.
  [tomashavlas]

v1.2
----

*Released: 2016-07-08*

- Refactored tests.
  [tomashavlas]

- Tagged tasks.
  [tomashavlas]

- Refactored tasks names.
  [tomashavlas]

- Replaced boolean string representations ('yes','true'/'no','false') with boolean values (true/false).
  [tomashavlas]

v1.1
----

*Released: 2016-06-30*

- Joined system group setup and remove tasks into single task.
  [tomashavlas]

- Created test case for root group.
  [tomashavlas]

- Added `trim` filter when checking for non-empty variables in conditions.
  [tomashavlas]

- Replaced complex conditions with `changed` and `failed` filters in acceptance tests.
  [tomashavlas]

- Updated minimal Ansible version to `2.0`.
  [tomashavlas]

- Replaced single line conditions with `ternary` filter.
  [tomashavlas]

v1.0
----

*Released: 2016-06-21*

- First public release
  [tomashavlas]
