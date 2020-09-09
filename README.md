# Tetration
Ansible Scripts for Tetration

Requirements

1. Ansible should be pre-installed on the control machine
2. Make sure ssh (username and password) and keys are available for Linux and Ubuntu servers.

Installation(with clear-text password)

$ git clone https://github.com/martin-charles/Tetration.git

1. Navigate to the main repository directory
2. Add your hosts to inventory file (inventory.ini)( this inventory will store password in clear text format)
3. Download sensors and put it into folder (/Tetration/roles/sensor_install/files)
4. There are two scripts a)to install pre-req b) to install actual sensor
5. Disable Host Key checking on the control machine (/etc/ansible/ansible.cfg)


User Guide
 
 -> Run the following command to install sensor on Centos/Redhat/Ubuntu machines
 
            ansible-playbook playbook.yml -i inventory.ini 


Installation(with ssh-keygen)

$ git clone https://github.com/martin-charles/Tetration.git

1. Generate ssh-keygen on the control machine
2. ssh-copy-id -i $HOME/.ssh/id_rsa.pub root@<server> (give the server password)
3. Add only hosts to inventory file (inventory_key.ini)
4. Download sensors and put it into folder (/Tetration/roles/sensor_install/files)
5. There are two scripts a)to install pre-req b) to install actual sensor
6. Disable Host Key checking on the control machine (/etc/ansible/ansible.cfg)

