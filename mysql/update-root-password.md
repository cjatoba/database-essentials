```bash
UPDATE mysql.user SET Password=PASSWORD('your_new_password') WHERE User='root';
OR IF ERROR
SET PASSWORD = PASSWORD('your_new_password');
```
