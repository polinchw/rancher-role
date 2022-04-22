Role Name
=========

Installs rancher on Ubuntu with docker-compose.  It will also install docker using a docker-role.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

```ansible-galaxy install -r requirements.yml```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

Example Playbook Commands
-------------------------

This will install docker, docker-compose, and rancher:

```ansible-playbook --private-key ~/.ssh/id_rsa -i tests/inventory tests/test.yml```

This will install docker and docker-compose:

```ansible-playbook --private-key ~/.ssh/id_rsa -i tests/inventory tests/test.yml --tags "docker"```

This will install rancher:

```ansible-playbook --private-key ~/.ssh/id_rsa -i tests/inventory tests/test.yml --tags "docker"```

This will install docker, docker-compose, and rancher and will override the location name:

```ansible-playbook --private-key ~/.ssh/id_rsa -i tests/inventory tests/test.yml --extra-vars "location=test user=polinchakb"```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
