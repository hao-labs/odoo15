# Quick install

Installing Odoo 15 with one command.

(Supports Odoo instances on one server)

Install [docker](https://docs.docker.com/get-docker/) and [docker-compose](https://docs.docker.com/compose/install/) yourself, then run:

# Usage

Start the container:
``` sh
docker-compose up
```

* Then open `localhost:10014` to access Odoo 15.0. If you want to start the server with a different port, change **10014** to another value in **docker-compose.yml**:

```
ports:
 - "10014:8069"
```

# Custom addons

The **addons/** folder contains custom addons. Put your custom addons if you have any.

# Odoo configuration & log

* To change Odoo configuration, edit file: **etc/odoo.conf**.
* Log file: **etc/odoo-server.log**

# Odoo container management

Run Odoo container in detached mode (be able to close terminal without stopping Odoo):

```
docker-compose up -d
```

**Restart Odoo**:

``` bash
docker-compose restart
```

**Start Odoo**:
``` bash
docker-compose start
```

**Stop Odoo**:

``` bash
docker-compose down
```

# docker-compose.yml

* odoo:15.0
* postgres:13
