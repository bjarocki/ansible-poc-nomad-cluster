## Setup
- `pip install ansible`
- `cat ~/.ansible.cfg`
```
[defaults]
roles_path = /your/home/ansible/roles
```
- `ansible-galaxy install -r roles.yaml`
- edit `poc` file and put your IPs
- `ansible -m ping all -i poc` to check if you can access your nodes
- `ansible-playbook -s ddance.yaml -i poc`
