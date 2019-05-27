# Note
- php-fpm version 7.0
- default port php-fpm-export : 9015
- connect to php-fpm via unix socket
step to run

- ansible-playbook file "install_php_nginx.yml"
- ansible-playbook file "enable_status" to set path status of php-fpm
- ansible-playbook file "php-fpm" to setup exporter

* default php-fpm-exporter will run as "www-data" user - same as php-fpm ( have to change if php-fpm run with different user)

ex command: ansible-playbook -i ~/Vagrant/network_1/hosts install_php_nginx.yml -e "host=master"


