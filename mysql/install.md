## Enable MySQL Repository:
```
sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2022 
```

## Install

In CentOS & RHEL 7:
```
sudo yum localinstall https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
sudo yum install mysql-community-server 
```

In Fedora 36:
```
sudo dnf install https://dev.mysql.com/get/mysql57-community-release-fc27-11.noarch.rpm
sudo dnf install mysql-community-server 
```

In Fedora 35:
```
sudo dnf install https://dev.mysql.com/get/mysql57-community-release-fc26-11.noarch.rpm
sudo dnf install mysql-community-server
```

Start Mysql service:
```
sudo systemctl start mysqld
```

Check temporary root password:
```
grep 'A temporary password' /var/log/mysqld.log |tail -1
```

## Configuration

Follow the wizard after execute mysql_secure_installation script:
```
/usr/bin/mysql_secure_installation
```

## Login

```
mysql -u root -p
```
