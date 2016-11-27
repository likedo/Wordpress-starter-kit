# Wordpress-starter-kit
Starting to develop a more complete kit with wordpress and git

## How to install

1. Download last release of Wordpress
2. Create /wordpress directory on FTP
3. Unzip Wordpress into /wordpress directory on FTP and install Wordpress
4. Set Wordpress core URL: http://yourdomain/wordpress or https://yourdomain/wordpress
5. Clone or download Wordpress Starter Kit and upload content into root FTP.
6. Into /wordpress directory on FTP, remove wp-content/, wp-config.php, .htaccess and index.php files
7. That's all folks :)

## How to use

1. Rename config-database-example.php to config-database.php
2. Rename wp-config-example.php to wp-config.php
3. Enter the connection data in config-database.php
4. Update security keys in wp-config.php - [generate key here](https://api.wordpress.org/secret-key/1.1/salt/):
 - define('AUTH_KEY',         'Put your unique phrase here');
 - define('SECURE_AUTH_KEY',  'Put your unique phrase here');
 - define('LOGGED_IN_KEY',    'Put your unique phrase here');
 - define('NONCE_KEY',        'Put your unique phrase here');
 - define('AUTH_SALT',        'Put your unique phrase here');
 - define('SECURE_AUTH_SALT', 'Put your unique phrase here');
 - define('LOGGED_IN_SALT',   'Put your unique phrase here');
 - define('NONCE_SALT',       'Put your unique phrase here');
5. Change the prefix of the table in wp-config.php, if you have changed during the installation of Wordpress
    - $table_prefix  = 'wp_';
