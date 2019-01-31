koichirok.chromedriver
=========

Ansible role to install chromedriver

Role Variables
--------------

See [defaults/main.yml](./defaults/main.yml)

variable | default | description
---------|---------|------------
chromedriver\_install\_prefix| /opt/google/chromedriver | The path where the chromedriver is installed. chromedriver executable is installed at {{chromedriver\_install\_prefix}}/bin|
chromedriver\_install\_as\_service | `false` | TBD |
chromedriver\_service\_state| not defined | TBD |
chromedriver\_service\_enabled| not defined | TBD |
chromedriver\_service\_user| ansible\_user\_uid | TBD |
chromedriver\_service\_group| ansible\_user\_gid | TBD |

Dependencies
------------

- koichirok.google\_chrome

Example Playbook
----------------

```
- hosts: servers
  roles:
     - koichirok.chromedriver
```

License
-------

BSD
