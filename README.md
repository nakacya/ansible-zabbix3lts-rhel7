
# Installation for Zabbix4 

clone repository
```
git clone https://github.com/nakacya/ansible-zabbix3lts-rhel7.git
```

configuration
```
vim ./ansible-zabbix-rhel7/group_vars/zabbix3lts-server-mysql-standalone
```

place of installation
```
vim ./ansible-zabbix4-rhel7/hosts
```

execute
```
cd ansible-zabbix3-rhel7
ansible-playbook -u <userName> ./zabbix3lts-server-mysql-standalone.yml

# public key authentication
ansible-playbook --private-key=<pathToPrivatekey> -u <userName> ./zabbix3lts-server-mysql-standalone.yml
```


First time login
```
http://<ipAddress or DNS>/zabbix/
user: Admin
pass: zabbix
```
#ansible-zabbix3lts-rhel7
