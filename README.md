OpenProject Configuration
=========================

Ready to use OpenProject docker-compose configuration for a traefik web proxy.

OpenProject is a web based project management sofware.

* OpenProject web page: https://github.com/hackmdio/codimd
* OpenProject docker description: 


Install
-------

```
# clone repository
git clone git@gitlab.wachter-jud.net:docker/openproject.git

# copy and edit the sample configuration file
cd openproject
cp docker-compose.yml.sample docker-compose.yml
```

Edit docker-compose.yml and change the following value:

* `YourSecretKey` create a new secret key
* `your.openproject.domain` define your public domain


First Startup
-------------

After the first startup login with the username: `admin` 
and password: `admin`.
You will then be asked by the system to change your administrative 
pasword.


Usage
-----

```
# start OpenProject
docker-compose up -d

# stop OpenProject
docker-compose down

# upgrade container
docker-compose pull
```



