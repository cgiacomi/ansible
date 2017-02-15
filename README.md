# Ansible

Sample ansible tasks


ansible-playbook -i inventory/development playbook-provision.yml


## Variables

- ssh_port: 22
- allowed_users: demo
- user_name: demo vagrant

password generation should be run on a similar machine, macOS does not create the correct value
python -c 'import crypt; print crypt.crypt("hello", "$1$SomeSalt$")'

- user_password: $1$SomeSalt$L9W/KYWMIdn7AfcMZZVeU0


set_fact: ansible_ssh_port={{ newsshport }}
//https://gist.github.com/chrisblossom/8690833
