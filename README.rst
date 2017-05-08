mrgall dokku host
=================
This is a set of ansible playbooks for controlling new dokku host.


Prerequisites:
--------------

.. code:: shell
   :number-lines:

    $ pip install ansible

Run:
----

.. code:: shell
   :number-lines:

    $ ansible-playbook -i hosts --private-key=~/.ssh/id_rsa --user $USER site.yaml
