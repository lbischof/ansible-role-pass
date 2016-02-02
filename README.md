[![Build Status](https://travis-ci.org/lbischof/ansible-role-pass.svg?branch=master)](https://travis-ci.org/lbischof/ansible-role-pass)
[![Galaxy Role](https://img.shields.io/badge/ansible--galaxy-pass-blue.svg)](https://galaxy.ansible.com/lbischof/pass/)


Pass Ansible Role
====

[pass](http://www.passwordstore.org) is a very simple password store that keeps passwords inside gpg encrypted files inside a simple directory tree. The pass utility provides a series of commands for manipulating the password store, allowing the user to add, remove, edit, synchronize, generate, and manipulate passwords.


Requirements
------------

None

Role Variables
--------------

```
pass_version: 1.6.5
pass_gpg_key: AFBA32A6
pass_git_remote: kexec.com:pass-store
```

Example Playbook
----------------

```
- hosts: servers
  roles:
    - lbischof.pass
```

License
-------

MIT
