## Create user

```bash
mysql> CREATE USER 'db_user'@'localhost' IDENTIFIED BY 'password';
```

## GRANT Permission to User on Database

```bash
mysql> GRANT ALL ON mydb.* TO 'db_user'@'localhost';
```

## Reload Privileges

```bash
mysql> FLUSH PRIVILEGES;
```

## Remove user

```bash
mysql> DROP USER db_user;
```
