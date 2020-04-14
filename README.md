Ansible user
=========

This is a wrapper role over [robertdebock.users](https://galaxy.ansible.com/robertdebock/users) in order to use it within the overall platform

Requirements
------------

Run `./configure` in order to download the role dependency. Also of course install Ansible :-).

Role Variables
--------------

Exactly the same as [robertdebock.users](https://galaxy.ansible.com/robertdebock/users): this role is totally dumb.
In addition to that roles variables, we have added the notion of system users, ex:

```yaml
    systemusers_user_list:
      - name: systemuser
        group: cmordante
        groups: wheel
        create_home: yes # defaults to false
        home: "/system" # defaults to "/" 
```

Dependencies
------------

[robertdebock.users](https://galaxy.ansible.com/robertdebock/users)


License
-------


[Apache-2](https://www.apache.org/licenses/LICENSE-2.0)

Author Information
------------------

* Twitter [@tcharl](https://twitter.com/Tcharl)
* Github [@tcharl](https://github.com/Tcharl)
* LinkedIn [Charlie Mordant](https://www.linkedin.com/in/charlie-mordant-51796a97/)
