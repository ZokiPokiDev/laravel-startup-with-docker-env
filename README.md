# Starting Laravel 7 App

## Docker-compose
    - php:7.4.3-fpm
    - nginx
    - mysql 8
    - phpmyadmin
    - nodejs:12
    
## Possibly a security precaution. You could try adding a new administrator account:

```mysql
mysql> CREATE USER 'monty'@'localhost' IDENTIFIED BY 'some_pass';
mysql> GRANT ALL PRIVILEGES ON *.* TO 'monty'@'localhost'
    ->     WITH GRANT OPTION;
mysql> CREATE USER 'monty'@'%' IDENTIFIED BY 'some_pass';
mysql> GRANT ALL PRIVILEGES ON *.* TO 'monty'@'%'
    ->     WITH GRANT OPTION;
```

Ready to go Laravel 7 app with docker integration!
