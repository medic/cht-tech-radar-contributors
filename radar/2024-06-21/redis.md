---
title:      "Redis"
ring:       stop
quadrant:   platform
tags:       [data]
---

[Redis](https://redis.io/) is an open source in-memory data store that can be used as a database, cache, or message broker.

In the context of the [CHT Sync](https://github.com/medic/cht-sync), Redis, in combination with Logstash was assessed for batching data changes from CouchDB to PostgreSQL.


It usage was discontinued in June 2024, as the combination of Redis, Logstash and PostgREST was not considered production-ready for various [reasons](https://github.com/medic/cht-sync/issues/107). CHT Sync uses an updated version of `couch2pg` to perform the sync between CouchDB and PostgreSQL.