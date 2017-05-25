# hello-forge-network

This repository contains an example of using forge to build and deploy
an entire network of services into kubernetes. The network consists of
4 services in total:

 - The *edge* service functions as an API gateway to the remaining
   three services: *products*, *ratings*, and *users*

 - The *products*, *ratings*, and *users* services are all simple
   stubs.

Connecting to <edge-ip>/<service-name> will access the corresponding
service by name.

## Repo Layout

Each of the four services is contained in a subdirectory of the
corresponding name. This is all contained within a single repo for
easy reference, however each service is deployed independently. (This
is essentially the monorepo pattern.) In practice forge can be used
with a monorepo layout like this, or forge can also be used on
services in separate repos, or even with a mix of the two approaches.
