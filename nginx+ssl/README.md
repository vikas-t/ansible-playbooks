### Ansible playbook to install nginx and configure SSL via Let's encrypt

Follow the steps to get it up and running 

1. Git clone the repo
2. Add your servers in hosts file
3. Replace variable according to your environment in roles/ssl/vars/main.yml
4. Use the following command to run the playbook 
  - `ansible-playbook -i hosts -u <your_remote_user> main.yml` 

####  Note :
1. Please note that the playbook runs only on Ubuntu and has been tested on Ubuntu 14.04
2. Lets Encrypt role is written to work only in *webroot* mode and not in the *standalone* mode


