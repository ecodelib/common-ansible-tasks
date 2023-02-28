# Common Ansible Tasks.
*This repo contains Ansible task modules performing some common tasks for both Debian and Redhat families...*

## Prerequisites
1. Hosts IP addresses should be listed in hosts.txt file.
2. Ansible should be installed on a control node (machine that runs Ansible and manages other nodes).
3. The procedure of generating an SSH key pair should be done. The public key to be copied to the hosts and installed in an authorized_keys file.

## Additional Info
Presented scripts were tested with Yandex Cloud platform services.  
Tasks involved in playbook:
- Check and print OS family 
- Disable password authentication
- Enable public key authentication
- Install Apache on different OS families with registering and printing debug info
- Generate index.html using Jinja template
- Copy files with loop
- Restart Apache if needed