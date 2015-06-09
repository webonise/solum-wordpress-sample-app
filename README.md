Example Wordpress Application
=============================


Pre-Requisites:
---------------

1. A database user
2. An existing database (defaults to wordpress)

Parameters to set:
------------------

* WORDPRESS_DB_HOST: <hostname>:3306
* WORDPRESS_DB_PASSWORD: <password>
* WORDPRESS_DB_USER: <user>
* WORDPRESS_DB_NAME: <wordpress_db>

To execute:
-----------

Set the above variables in params.yaml

```
solum app create --git-url https://github.com/rackspace-solum-samples/solum-wordpress-sample-app --lp wordpress422 --run-cmd ./start.sh  --name wordpress-app --port 80 --param-file params.yaml
```

NOTE: make sure your user has access to the db. Else, you get errors.

