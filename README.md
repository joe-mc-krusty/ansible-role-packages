Ansible Role: Packages
=========

An Ansible role for managing packages with the package module (apt, yum, etc)

Requirements
------------

None

Role Variables
--------------

```yaml
packages:
  - name: zsh
    state: present
  
  - name: vim
    state: latest 
    use: "apt"
```
See [Ansible Package Module Documentation](https://docs.ansible.com/ansible/latest/modules/package_module.html) to know more about parameters.

Dependencies
------------

None

Example Playbook
----------------


    - hosts: servers
      roles:
         - joe_mc_krusty.packages

License
-------

BSD

Author Information
------------------

Maintained by Xavier Sanna
