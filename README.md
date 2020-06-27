Cryptpad Configuration
=======================

Ready to use cryptpad docker-compose configuration for a traefik web proxy.

Cryptpad is an encrypted collaborative editor for rich text, markdown,
kanban boards, todo lists and polls.

cryptpad project: hhttps://cryptpad.fr/


Install
-------

Clone and edit repository:

```
# clone repository
git clone git@gitlab.wachter-jud.net:docker/cryptpad.git

# copy and edit the sample configuration file
cd cryptpad
cp docker-compose.yml.sample docker-compose.yml
cp config.js.sample config.js
```

Edit `docker-compose.yml` and change the following value:

* `your.cryptpad.domain` the domain name under which this cryptpad will be available


Optionally edit `config.js` and change the following values:

* adminEmail: "your@email"
* httpSafeOrigin: "https://your.domain",


Usage
-----

```
# start nextcloud
docker-compose up -d

# stop nextcloud
docker-compose down
```


