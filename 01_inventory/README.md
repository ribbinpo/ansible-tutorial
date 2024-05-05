# Test Command (Ping)

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