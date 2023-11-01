Role Name
=========
__linuxptp__ Deploy linuxptp on Linux KVM Virtual machines in FABRIC Project setup.

Requirements
------------
- Requires Ansible 2.9 or greater (on the Ansible command center)
- Currently supported Operating system(destination machines) are 
  - Ubuntu 18.04 or greater
  - CentOS 8 or greater

Example Playbook
----------------
<pre>
  - hosts: all
    roles:
      role: linuxptp
</pre>          

Example Run
----------------
<pre>

ansible-playbook -i <INVENTORY_FILE> playbook_fabric_experiment_ptp.yml

ansible-playbook -i <INVENTORY_FILE> playbook_fabric_experiment_ptp.yml --extra-params @parameters.json

ansible-playbook -i <INVENTORY_FILE> playbook_fabric_experiment_ptp.yml --tags=ptp_install

ansible-playbook -i <INVENTORY_FILE> playbook_fabric_experiment_ptp.yml --tags=ptp_start

ansible-playbook -i <INVENTORY_FILE> playbook_fabric_experiment_ptp.yml --tags=ptp_stop
</pre>          
License
-------

BSD

Author Information
------------------

Hussamuddin Nasir
(nasir@netlab.uky.edu)
