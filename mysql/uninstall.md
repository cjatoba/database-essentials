In CentOS e RedHat:
```
sudo yum remove mysql mysql-server
```
 
Para usuários do Ubuntu e Debian:
```
sudo apt remove mysql mysql-server
```
 
In Fedora:
```
sudo dnf remove mysql mysql-server
```

Rename ou remove mysql folder (Rename for backup data):
```
sudo mv /var/lib/mysql /var/lib/mysql_directory_backup
Or
sudo rm -rf /var/lib/mysql /var/lib/mysql_directory_backup
```
