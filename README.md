Ansible Wordpress
--------

Ansible Role that installs WordPress

## Dependencies

    geerlingguy.apache 
    geerlingguy.php 

## Example Playbook

    ---
    - hosts: webservers
      roles:
        - { role: robruma.wordpress }
      vars:
        wordpress_db_name: wordpress
        wordpress_db_user: admin
        wordpress_db_host: localhost
        wordpress_db_password: secret
        wordpress_site_name: blog.site.org
