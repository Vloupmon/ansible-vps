# ansible-vps
My Oracle (OCI) VPS's Ansible conf.

Currently deploying :
- Docker
- Caddy
- Drone
- Filebrowser

As well as doing some miscellaneous file operations.

`ansible-playbook` needs the hostname envar, the SSH parameters, as well as the flag necessary to request the vault password.

The command looks like `ansible-playbook -v -i hosts -u ssh_user --private-key /path/to/key --extra-vars '{"hostname":"something.com"}' --ask-vault-pass --diff playbooks/vps.yml`
