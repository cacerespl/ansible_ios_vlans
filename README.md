# ansible_ios_vlans
Create Voice and Data vlans and assign them to a port by using Jinja2 template with Ansible

# Running the playbook
ansible-playbook -i hosts vlan_configuration.yml 

**This playbook will create:**
- Some users to the local database
- Two Vlans (Voice and data) with their names
- Assign the voice and data vlans to some ports

**The Playbook perform two tasks:**
  - The first task is to generate a configuration file (*conf.cfg*) and add it to the current directory
  - The second task is to deploy the configuration by using the file generated previously

All the variables are defined inside group_vars/all.yml file.
