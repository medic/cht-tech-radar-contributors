---
title:      "dbt"
ring:       adopt
quadrant:   tools
tags:       [data]
---

[dbt](https://www.getdbt.com/) uses SQL to model simple batch transformations, while it provides command-line tooling that encourages good engineering practices such as versioning, automated testing and deployment; essentially it implements SQL-based transformation modeling as code. It currently supports multiple data sources, including PostgreSQL.

It the CHT context, dbt runs data tests and migrations for [CHT Sync](https://github.com/medic/cht-sync). Once CouchDB data is synchronized and stored in PostgreSQL with CHT Sync, it undergoes transformation using predefined dbt models from the [cht-pipeline repository](https://github.com/medic/cht-pipeline). dbt is used to ingest raw JSON data from the PosgtreSQL database and normalize it into a relational schema to make it easier to query.

You can find more details about CHT data synchronization tools [in the related documentation](https://docs.communityhealthtoolkit.org/core/overview/cht-sync/).
