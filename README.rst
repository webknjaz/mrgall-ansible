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

    $ pip install 'ansible>=2.5.0'
    $ vim .vault_pass  # ask for it from someone who has it

Run:
----

.. code:: shell
   :number-lines:

    $ ansible-playbook site.yaml -e "ansible_ssh_private_key_file=~/.ssh/id_rsa ansible_ssh_user=$USER"
