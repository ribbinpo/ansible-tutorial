# Ansible Variable

## Integrate variable with db playbook
```bash
ansible-playbook -i inventory playbooks/db.yaml
# -v  for provides more information than the default output
# -vv for deep troubleshooting and debugging scenarios where need information about Ansible's internal operations
```

## For playbook testing
```bash
ansible-playbook -i inventory playbooks/vartest.yaml
# -v  for provides more information than the default output
# -vv for deep troubleshooting and debugging scenarios where need information about Ansible's internal operations
```

