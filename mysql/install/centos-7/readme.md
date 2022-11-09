- Install the Percona yum repository by running the following command as a root user or with sudo:

```bash
sudo yum install https://repo.percona.com/yum/percona-release-latest.noarch.rpm
```

- Enable the Percona Server 5.7 repository:
```bash
sudo percona-release setup ps57
```

- Install the packages. You can install Percona Server for MySQL by running the following command:
```bash
sudo yum install Percona-Server-server-57
```

- Start the service. Percona Server for MySQL does not start automatically on RHEL and CentOS after the installation. Start the server by running the following command:
```bash
sudo service mysql start
```

Credits: https://docs.percona.com/percona-server/5.7/installation/yum_repo.html
