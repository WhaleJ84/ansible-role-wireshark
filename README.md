wireshark
=========

Installs and configures wireshark.

Requirements
------------

This role has no requirements.

To include this role in your `requirements.yml` file, add the following list item:

```yaml
---
roles:
  - name: whalej84.wireshark
    src: https://github.com/whalej84/ansible-role-wireshark.git
    scm: git
```

The role can then be installed using `ansible-galaxy install -r requirements.yml whalej84.wireshark`.

Role Variables
--------------

See [defaults](./defaults/main.yml).

Example Playbook
----------------

This exmaple playbook shows how I would use this role, with custom variables to suit my needs:

```yaml
---
- hosts: localhost

  roles:
    - role: whalej84.wireshark
      tags: [wireshark]
```
