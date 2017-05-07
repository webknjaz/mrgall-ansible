yoshz.dokku
===========

An Ansible role for installing [dokku](https://github.com/progrium/dokku).


Requirements
------------

* Docker should be installed ([yoshzz.docker](https://github.com/yoshz/ansible-role-docker))


Role Variables
--------------

Configure different vhost:

    dokku_vhost: example.com

Install plugins:

    dokku_plugins:
      - { name: "docker-options", repo: "https://github.com/dyson/dokku-docker-options.git" }


Dependencies
------------

None


License
-------

MIT
