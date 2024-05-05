# Test Command (Ping)

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