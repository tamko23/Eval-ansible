# Eval-ansible



retour de commande:
ansible_ipi) ansible@ip-10-0-103-38:~$ ansible-playbook -i inventory.ini create_ressource.yml 
[DEPRECATION WARNING]: community.general.yaml has been deprecated. The plugin has been superseded by the the option `result_format=yaml` in callback plugin ansible.builtin.default from ansible-core 2.13 onwards. This feature will be 
removed from community.general in version 13.0.0. Deprecation warnings can be disabled by setting deprecation_warnings=False in ansible.cfg.

PLAY [Create Azure VM] **********************************************************************************************************************************************************************************************************************

TASK [Gathering Facts] **********************************************************************************************************************************************************************************************************************
[WARNING]: Platform linux on host localhost is using the discovered Python interpreter at /home/ansible/ansible_ipi/bin/python3.13, but future installation of another Python interpreter could change the meaning of that path. See
https://docs.ansible.com/ansible-core/2.18/reference_appendices/interpreter_discovery.html for more information.
ok: [localhost]

TASK [Create resource group] ****************************************************************************************************************************************************************************************************************
ok: [localhost]

TASK [Create virtual network] ***************************************************************************************************************************************************************************************************************
ok: [localhost]

TASK [Add subnet] ***************************************************************************************************************************************************************************************************************************
ok: [localhost]

TASK [Create public IP address] *************************************************************************************************************************************************************************************************************
ok: [localhost]

TASK [Public IP of VM] **********************************************************************************************************************************************************************************************************************
ok: [localhost] => 
  msg: The public IP is 52.142.62.83.

TASK [Create Network Security Group that allows SSH] ****************************************************************************************************************************************************************************************
ok: [localhost]

TASK [Create virtual network interface card] ************************************************************************************************************************************************************************************************
ok: [localhost]

TASK [Create VM] ****************************************************************************************************************************************************************************************************************************
changed: [localhost]

PLAY RECAP **********************************************************************************************************************************************************************************************************************************
localhost                  : ok=9    changed=1    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

(ansible_ipi) ansible@ip-10-0-103-38:~$ 

![image](https://github.com/user-attachments/assets/4cfe2bda-4cc6-47ed-ae9c-d090620d0ac0)
