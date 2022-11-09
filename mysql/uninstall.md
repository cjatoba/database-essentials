In CentOS e RedHat:
```bash
sudo yum remove mysql mysql-server
```
 
Para usuários do Ubuntu e Debian:
```bash
sudo apt remove mysql mysql-server
```
 
In Fedora:
```bash
sudo dnf remove mysql mysql-server
```

Rename ou remove mysql folder (Rename for backup data):
```bash
sudo mv /var/lib/mysql /var/lib/mysql_directory_backup
Or
sudo rm -rf /var/lib/mysql
```
