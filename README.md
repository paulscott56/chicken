chicken
=======

NodeJS hacks for a bigData stats server

This project is based on Hummingbird, which can be found at https://github.com/mnutt/hummingbird


Description
---------------

Chicken tracks sites by GET request.


Requirements
-------------------

 * node.js v0.6.16
 * npm v1.1.19
 * mongodb v2.0.4


Installation
--------------

    # Use npm to install the dependencies
    npm install

    # Copy the default configuration file
    cp config/app.json.sample config/app.json

    # To use the map, download MaxMind's GeoIP database and extract to the root directory:
    wget http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz
    gunzip GeoLiteCity.dat.gz


Running Chicken
-----------------------------

To start the analytics server, run the following:

    mongod (or start mongo some other way)
    node server.js

By default a dashboard will be run on port 8080
