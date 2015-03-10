ansible-cozy-playbook
=====================

Short playbook to show how ansible-cozy-role can be used on an existing server.

Requirements
------------

This playbook requires Ansible 1.4 or higher. It has been tested on Debian 7 and Ubuntu 14.04.

Another requirements:
- NodeJS role from [AnsibleShipyard/ansible-nodejs](https://github.com/AnsibleShipyard/ansible-nodejs)
- CouchDB role from [guillaumededrie/ansible-role-couchdb](https://github.com/guillaumededrie/ansible-role-couchdb)
- Cozy role from [Kloadut/ansible-cozy-role](https://github.com/Kloadut/ansible-cozy-role)


Installation
------------

Run:
```
$ ansible-galaxy install -r galaxy.yml -p ./roles
```

Execution
---------

Run:
```
$ ansible-playbook playbook.yml
```

You can add those two options, to activate debug and to set a FQDN for the certificate generation
```
$ ansible-playbook playbook.yml -vvvv -e ansible_fqdn=cozy.test.me
```


Licence
-------

GNU GPL v2
