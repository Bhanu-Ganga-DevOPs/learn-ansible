ansible-pull :
To run the ansible yml file from GITHub repo url to local the receiver server in which ansible installed we use ansible-pull command
Ex : ansible-pull -i localhost, -u GitHUbURl

Ansible ad-hoc command example
1. ansible -i /tmp/inv all -U ansible_username=centos ansible_password=