# Ansible - To Install Wordpress 

## Playbook to setup  
- Mariadb Server
- Nginx
- PHP
- Wordpress

##  Files

  -  wordpress_nginx.yaml
  - wp-config.php.tmpl
  - vhost_temp.tmpl
  - wp.vars
  - hosts
 
#  wp.vars
All variables declared on this file

### 12 tasks
  -  Upgrade all apt packages
  -  Install required packages
  - Install mysql-python package
  - Write root login credentials
  - Set root user password
  - Create database
  - Create extra user
  - Create website configuration file
  - create soft link for the website
  - Create website folder
  - Download wordpress tar file to tmp folder
  - Untar the file
  - copy wordpress files from tmp folder to document root
  - Update wp-config file
  - Unlink the default configuration file
  - Restart nginx service

## Folder
Websie folder name: wordpress

## vhost_temp.tmpl
Website template configuration file

## wp-config.php.tmpl
wp-config.php file template with updated database connection string

