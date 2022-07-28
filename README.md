# Ansible-Playbook-Deploy-ALDPro
Ansible playbook for deploying and configuring ALD Pro Domain Controller and other servers with roles

Supported platforms
------------

##### Astra Linux
*  1.7

Playbook Variables
--------------
Please see vars in deploy-aldpro.yml and inventory files

You can also use tags: 

*  __first_dc__ - deploy first Domain Controller
*  __client-server__ - deploy aldpro client to servers from ALD Pro role 
*  __client__ - deploy aldpro client to clients

Dependencies
------------

* None

Example 
----------------

__ansible-playbook -l dc01 deploy-aldpro.yml --tags="first_dc"__ - deploy first Domain Controller

__ansible-playbook -l repo deploy-aldpro.yml --tags="client-server"__ - deploy aldpro client to servers ALD Pro role

__ansible-playbook -l client-1 deploy-aldpro.yml --tags="client"__ - deploy aldpro client to clients

License
-------

MIT

Author Information
------------------

Aleksandr Anishchenko
