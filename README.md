ansible-pull :
To run the ansible yml file from GITHub repo url to local the receiver server in which ansible installed we use ansible-pull command
Ex : ansible-pull -i localhost, -u GitHUbURl

Ansible ad-hoc command example
1. ansible -i /tmp/inv all -e ansible_username=centos -e ansible_password=***** abc.yml

Ansible variables 
1. Variable are accessed as {{ variable_name }}
2. Ansible supports both double and single quotes
3. If a value starts with variable the quote are mandatory other wise not mandatory 
   1. Play level Variables are accessible with in all the tasks under that play
   2. 