Veilid
======

This Ansible role allows you to quickly set up headless Veilid nodes. The target system is configured to automatically update and restart when necessary.

Supported platforms
-------------------

This role has been tested against Debian (Bookworm, Bullseye, Buster) and Ubuntu (Jammy). 

Example Playbook
----------------

The Veilid role is quite simple and requires no configuration. An example playbook would be:

```
---
- hosts: all
  remote_user: root
  roles:
    - solace_10.veilid
```

If you're using an inventory, you can run the playbook with:

```
ansible-playbook -i path/to/your/inventory path/to/your/playbook.yml
```

If you don't want to use an inventory, you can run the playbook explicity against one or more targets (note that if running against a single target, you need the comma after IP):

```
ansible-playbook -i 68.133.118.91, path/to/your/playbook.yml
```

License
-------

This role is under the MIT license.

Author Information
------------------

This role has been developed by Pedro Nunes (Solace-10). If you have issues or suggestions regarding this role, please use the GitHub issues page.
