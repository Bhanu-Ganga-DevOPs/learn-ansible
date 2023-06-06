ansible-pull :
To run the ansible yml file from GITHub repo url to local the receiver server in which ansible installed we use ansible-pull command
Ex : ansible-pull -i localhost, -u GitHUbURl

Ansible ad-hoc command example
1. ansible -i /tmp/inv all -e ansible_username=centos -e ansible_password=***** abc.yml

**Ansible variables** 
1. Variable are accessed as {{ variable_name }}
2. Ansible supports both double and single quotes
3. If a value starts with variable the quote are mandatory other wise not mandatory 
   1. Play level Variables are accessible with in all the tasks under that play
   2. Variable taken from files into playbook are accessible to plays not constrained to individual tasks(task level).
4. Variables Precedence
   1. Variables from CLI
   2. Variables from tasks
   3. Variables from roles
   4. Variables from files
   5. Variables from plays
   6. Variables from Inventory
   7. Variables from defaults
5. Variables from one task to another task can be done using "register" keyword