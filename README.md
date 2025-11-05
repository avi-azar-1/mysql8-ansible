# mysql8-ansible

generic install for mysql8 instance on rhel 8 servers, including software unpacking and creation of service and conf files

**HOW TO**

1. **downloads**:  
- download this repo  
- also download ansible rhel 8 install from:  
https://github.com/avi-azar-1/rhel8.8-ansible

2. **install ansible**:  
look at instructions in ansible repo

3. **ready mysql install**:  
unzip this repo in target server  

4. **edit playbook**:  
change target server and parameters inside mysql_inventory.yaml

5. **run playbook**:  
from playbook folder:
```bash
ansible-playbook -i mysql_inventory.yaml installmysql.yaml
```
for local install (without ssh) run with '-c local' flag  
for remote ssh create id_rsa.pub in ansible server and copy to known_hosts un target server  



