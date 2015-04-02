# c9couch
Access to CouchDB Futon from Cloud9 IDE for Node.JS project

Cloud9 IDE does not provide a way to access to Futon - web admin interface to CouchDB. This script do nothing but forward http requests to couchdb. It helps to work with Futon.

## Use

Setup CouchDB

    sudo mkdir -p /var/run/couchdb
    sudo chown couchdb:couchdb /var/run/couchdb 

Start CouchDB
    
    sudo su couchdb -c /usr/bin/couchdb

Run script

    node c9couch.js
    
Now you can access Futon from web browser at **/_utils/** (Ex.: https://c9couch-username.c9.io/_utils/ )
