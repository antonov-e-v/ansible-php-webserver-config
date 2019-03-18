# ansible-php-webserver-config
Configure webserver for PHP application via Ansible

It will install:

- Fail2ban
- Ufw
- Php with some needed extensions
- Nginx
- MariaDB
- Git
- Composer
- Python-mysqldb

It will create:

- User with name `webmaster` and password `password` (don't forget to change it in `vars` parameters)
- Database with name `app_db`
- Database user with name `app_user` and password `app_user_password` (don't forget to change it in `vars` parameters) and all priveleges to `app_db`

It will configure:
- Nginx config and site template for site `example.com` (don't forget to change it in `vars` parameters)
- Php-fpm config

This configuration successfully tested with Laravel 5.8
