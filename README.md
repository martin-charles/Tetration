# Tetration
Ansible Scripts for Tetration

Requirements

1. Ansible should be pre-installed on the control machine
2. Make sure ssh (username and password) and keys are available for Linux and Ubuntu servers.

Installation

$ git clone https://github.com/martin-charles/Tetration.git

1. Navigate to the main repository directory
2. Add your hosts to inventory file (inventory.ini)
3. Download sensors and put it into folder (/Tetration/roles/sensor_install/files)
4. There are two scripts a)to install pre-req b) to install actual sensor

User Guide
 Run the following command to install sensor on Centos/Redhat/Ubuntu machines
 
 ansible-playbook playbook.yml -i inventory.ini
