## Plugin development

- move your `your-plugin-directory` into `wordpress-docker` directory (root of this folder)
- edit `$ vim/nano docker-compose.yml` file and replace `{plugin-directory}` by `your-plugin-directory`

- Start docker `$ docker-compose up`.
- Wordpress should be on `http://localhost:8080`, and setup basic configuration.
- Access to PHPMyAdmin is on `http://localhost:8181`
- log in as admin and open `plugins`, find `your-plugin-NAME` and enable.


Your plugin name is on root plugin file in comment 
```
<?php
/*
  Plugin Name: your-plugin-NAME
  Plugin URI: your-plugin-URL
  Description: your-plugin-DESCRIPTION
  Version: 1.0
  ... rest of field on WP documentation
*/
?>

```

