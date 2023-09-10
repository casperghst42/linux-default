# Ansible setup 

This is for my own use, there are quite curtain better ways to do this, but it works for me.

To configure a server to my likings.

1) setup vault and variables in roles/defaults (read the sample files)

2) run bootstrap<br/>
ansible-playbook bootstrap.yml -i &lt;ip>, -extra-vars "ansible_ssh_user=${USER}"  --ask-become-pass --ask-pass

3) run everything<br/>
ansible-playbook xyz.yml -i &lt;ip>, --ask-vault-pass  --ask-pass --ask-become-pass

