# Ansible
Ansible Useful Commands

## Ansible Modules
Ansible **modules** are reusable, standalone scripts that can be used by the Ansible API, or by the ansible or ansible-playbook programs. They return information to ansible by printing a JSON string to stdout before exiting.

Module usage example: 
```markdown
$ ansible <ansible_host> -m <module_name>
```

### Module > Ping 
```markdown
# ping module for all hosts
$ ansible -m ping all

# ping module for ansible localhost 
$ ansible -m ping	localhost	# ping localhost
$ ansible -m ping	<host>
```

### Module > Setup
```markdown
# setup module for localhost ansible
$ ansible localhost -m setup		# show ansible facts for localhost
```
