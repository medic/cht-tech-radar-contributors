---
title:      "PostgREST"
ring:       stop
quadrant:   tools
tags:       [data]
---

[PostgREST](https://postgrest.org/en/v12/) acts as a RESTful API layer, by providing endpoints to store and retrieve the data in/from a PostgreSQL database.

In the context of the CHT, PostgREST, in combination with Logstash and Redis was assessed for synching data from CouchDB to PostgreSQL in [CHT Sync](https://github.com/medic/cht-sync). 

It usage was discontinued in June 2024, as Logstash was not considered production-ready for various [reasons]. CHT Sync uses an updated version of `couch2pg` to perform the sync between CouchDB and PostgreSQL.