## The Edge Service

The edge service is a simple API gateway implemented in
flask. Typically your API gatway would sit at the edge of a network of
services and provide any cross-cutting or custom logic needed by the
rest of the network. Examples of this might include authentication and
authorization, global rate limiting, content based routing, and more.
