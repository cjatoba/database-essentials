## Create user

```bash
mysql> CREATE USER 'db_user'@'localhost' IDENTIFIED BY 'password';
```

## Create user with grant option:

```bash
GRANT ALL ON *.* TO 'db_user'@'%' IDENTIFIED BY 'password' WITH GRANT OPTION;
```
