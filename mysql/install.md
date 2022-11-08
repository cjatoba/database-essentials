

## Install

In Ubuntu:

```bash
wget https://dev.mysql.com/get/mysql-apt-config_0.8.12-1_all.deb
sudo dpkg -i mysql-apt-config_0.8.12-1_all.deb
```

- In prompt select below options:
> select Ubuntu Bionic
> After that, select the MySQL Server & Cluster option. Then, select mysql-5.7 and finally select Ok

- update the APT repository:
```bash
sudo apt update
```

- If you encounter the "signature couldn't be verified" error like this one: NO_PUBKEY 467B942D3A79BD29, you will need to import the missing gpg key by running the following command:
```bash
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 467B942D3A79BD29
sudo apt update
```

- To check whether MySQL 5.7 repository has been successfully installed, execute:
```bash
sudo apt-cache policy mysql-server
```

- Install mysql 5.7:
```bash
sudo apt install -f mysql-client=5.7* mysql-community-server=5.7* mysql-server=5.7*
```

- Press Y to begin the installation and set the root password when asked

In CentOS & RHEL 7:
```bash
sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2022 
sudo yum localinstall https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
sudo yum install mysql-community-server 
```

In Fedora 36:
```bash
sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2022 
sudo dnf install https://dev.mysql.com/get/mysql57-community-release-fc27-11.noarch.rpm
sudo dnf install mysql-community-server 
```

In Fedora 35:
```bash
sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2022 
sudo dnf install https://dev.mysql.com/get/mysql57-community-release-fc26-11.noarch.rpm
sudo dnf install mysql-community-server
```

Start Mysql service:
```bash
sudo systemctl start mysqld
```
