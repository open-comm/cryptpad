Cryptpad Configuration
=======================

Ready to use cryptpad docker-compose configuration for a traefik web proxy.

Cryptpad is an encrypted collaborative editor for rich text, markdown,
kanban boards, todo lists and polls.

cryptpad project: hhttps://cryptpad.fr/


Install
-------

Build docker image in a separate source directory

```
# clone cryptpad source
git clone https://github.com/xwiki-labs/cryptpad.git cryptpad-source
cd cryptpad-source

# build the docker image
docker build -t xwiki/cryptpad .
```

Clone and edit this repository else where, and start the image:

```
# clone repository
git clone git@gitlab.wachter-jud.net:docker/cryptpad.git

# copy and edit the sample configuration file
cd cryptpad
cp docker-compose.yml.example docker-compose.yml
```

Edit docker-compose.yml and change the following value:

* `your.cryptpad.domain` the domain name under which this cryptpad will be available




Usage
-----

```
# start nextcloud
docker-compose up -d

# stop nextcloud
docker-compose down
```


Udpate
------

Update the cryptpad source git repository and build a new docker image.

```
# move to the source git repository and get the latest source
git pull

# build a new docker image
docker build -t xwiki/cryptpad .
```



