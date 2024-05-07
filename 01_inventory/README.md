# Test Command

## Test inventory with ping

All servers

```bash
ansible all -m ping -i inventory
```

Speicific target server

```bash
ansible server01 -m ping -i inventory
```

Target group servers

```bash
ansible webservers -m ping -i inventory
```

Target server with regular expression

```bash
ansible 'server*' -m ping -i inventory
```

## Test AC HOC command

Example: service
```bash
ansible server01 -m ansible.builtin.apt -a "name=apache2 state=present update_cache=yes"
# add --become to be sudo
# state -> present, absent
```
Example: copy
```bash
# copy file
ansible server01 -m ansible.builtin.copy -a "src=index.html dest=/var/www/html/index.html"
```
