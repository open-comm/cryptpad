# Cryptpad Configuration

Ready to use cryptpad docker-compose configuration for a traefik web proxy.

Cryptpad is an encrypted collaborative editor for rich text, markdown,
kanban boards, todo lists and polls.

cryptpad project: hhttps://cryptpad.fr/


## Install

Clone and edit repository:

```
# clone repository
git clone https://git.open-communication.net/open-communication/docker/cryptpad.git

# move into project folder
cd cryptpad

# copy and edit the sample configuration files
cp sample.env .env
cp config.js.sample config.js
```

Edit environment configuration file `.env` and change the following values:

* `my.domain.com` the domain name under which this cryptpad will be available
* `Choose_A_Unique_Name` choose a name unique name for your cryptpad router.
  The name must not include spaces or dots.


Optionally edit `config.js` and change the following values:

* adminEmail: "your@email"
* httpSafeOrigin: "https://your.domain",


## Usage

```
# start cryptpad
docker-compose up -d

# stop cryptpad
docker-compose down

# upgrade container
docker-compose pull
```

