mrgall dokku host
=================
This is a set of ansible playbooks for controlling new dokku host.
To start copy id_rsa_mrgall SSH private key into this dir.


Prerequisites:
--------------

.. code:: shell
   :number-lines:

    $ pip install ansible

Run:
----

.. code:: shell
   :number-lines:

    $ ansible-playbook -i hosts site.yaml
