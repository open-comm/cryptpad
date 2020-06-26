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
cp docker-compose.yml.example docker-compose.yml
```

Edit docker-compose.yml and change the following value:

* `your.cryptpad.domain` the domain name under which this cryptpad will be available


In order to run cryptpad you need to configure the 'config.js' file in `data/config/config.js`. 

You need to set at least the following configuration:

* adminEmail: "your@email"
* httpSafeOrigin: "https://your.domain",
* httpAddress: '::',

Optionally change:

* defaultStorageLimit: 1024 * 1024 * 1024,
* blockDailyCheck: true,
* removeDonateButton: true,


Usage
-----

```
# start nextcloud
docker-compose up -d

# stop nextcloud
docker-compose down
```


