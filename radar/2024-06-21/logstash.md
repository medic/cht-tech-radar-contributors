---
title:      "Logstash"
ring:       stop
quadrant:   tools
tags:       [data]
---

[Logstash](https://www.elastic.co/logstash) is a free and open server-side data processing pipeline. It can ingest data from a multitude of sources, transforms it, and then sends it to a "stash."

In the context of the CHT, Logstash, in combination with [`logstash-input-couchdb_changes`](https://github.com/logstash-plugins/logstash-input-couchdb_changes/tree/main) was assessed for synching data from CouchDB to PostgreSQL in [CHT Sync](https://github.com/medic/cht-sync). 

It usage was discontinued in June 2024, as it was not considered production-ready for various [reasons]. CHT Sync uses an updated version of `couch2pg` to perform the sync between CouchDB and PostgreSQL.