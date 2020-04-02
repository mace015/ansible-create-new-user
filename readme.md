# ansible-create-new-user

NOTE: This playbook is meant to be used after running: [ansible-docker-webserver](https://github.com/mace015/ansible-docker-webserver)

This ansible playbook adds a new user with sudo, a random password and a authorized key.

## Usage

To use this setup run the following command:

`
ansible-playbook -i HOST, create-user.yml --private-key ~/.ssh/PRIVATE-KEY --extra-vars "user=USER authorized_key=~/.ssh/id_rsa.pub"
`