## Enable MySQL Repository:
```bash
sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2022 
```

## Install

In CentOS & RHEL 7:
```bash
sudo yum localinstall https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
sudo yum install mysql-community-server 
```

In Fedora 36:
```bash
sudo dnf install https://dev.mysql.com/get/mysql57-community-release-fc27-11.noarch.rpm
sudo dnf install mysql-community-server 
```

In Fedora 35:
```bash
sudo dnf install https://dev.mysql.com/get/mysql57-community-release-fc26-11.noarch.rpm
sudo dnf install mysql-community-server
```

Start Mysql service:
```bash
sudo systemctl start mysqld
```

Check temporary root password:
```bash
grep 'A temporary password' /var/log/mysqld.log |tail -1
```
