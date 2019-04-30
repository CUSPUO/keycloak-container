### Keycloak container image

Keycloak container image using MariaDB as persisted database.

#### Configure:

- Fill in the variables inside `keycloak_secret.env.sample` and `mariadb_secret.env.sample`.
- Rename them to `keycloak_secret.env` and `mariadb_secret.env` respectively
- This specific configuration requires 2 docker networks to exist on the system:
    - uonet-overlay
    - webproxy

#### Run:

- `docker-compose up -d`

**Optional**

This stack can also use the [nginx-revproxy](https://github.com/CUSPUO/nginx-revproxy) to serve
the requests over HTTPS
