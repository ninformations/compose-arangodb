# Docker compose for arangodb

* scaling works for DBs
* docker nginx proxy to connect to cordinator
* contains 1 agency, 3 coordinators, 1 db.

## How to run
run `docker-compose up --build`

and add following to etc/hosts
> 127.0.0.1 arango.local

and fire `arango.local` in browser

## for scaling run this

> `$ docker-compose scale db=<num>`

#### @TODOs
    * coordiantor scaling
    * nginx loadbalancing (KB: right now nginx-proxy isn't doing load balancing)
