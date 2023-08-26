# Ansible setup 

To configure a server to my likings.

1) setup vault and variables in roles/defaults (read the sample files)

2) run bootscrap<br/>
ansible-playbook bootstrap.yml -i <ip>, -extra-vars "ansible_ssh_user=${USER}" --ask-ssh-pass

3) run everything<br/>
ansible-playbook xyz.yml -i <ip>, --ask-vault-pass

