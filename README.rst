mrgall dokku host
=================
This is a set of ansible playbooks for controlling new dokku host.
To start copy id_rsa_mrgall SSH private key into this dir. Alternatively
override per-host vars as in example below.


Prerequisites:
--------------

Install ansible and drop a vault password file inplace:

.. code:: shell
   :number-lines:

    $ pip install 'ansible>2.3.1'
    $ vim .vault_pass

Run:
----

.. code:: shell
   :number-lines:

    $ ansible-playbook -i hosts site.yaml  -e "ansible_ssh_private_key_file=~/.ssh/id_rsa ansible_ssh_user=$USER"
