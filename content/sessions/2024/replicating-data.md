---
title: "Replicating data between transactional databases and ClickHouse®"
slug: designing-a-lakehouse-for-product-engineers
speakers:
 - Kanthi Subramanian
 - Arnaud Adant
topics:
 - Data ingestion
day: 20243
room: B
timeslot: 3
time_start: 2024-11-21T16:30:00.000Z
time_end:   2024-11-21T17:00:00.000Z
gridarea: 2/3/3/4
---

Transactional databases like MySQL, PostgreSQL and MongoDB are usually not a great fit for real time analytics, especially as the data volume grows.

They are also less space efficient than columnar databases and require regular purge or archival. This talk presents a solution to synchronize data in real time between MySQL and ClickHouse. The Altinity Sink Connector open source project (https://github.com/Altinity/clickhouse-sink-connector) is designed to efficiently replicate data and schema changes with accuracy, operational simplicity and performance in mind. It also provides tools to checksum and efficiently dump and load Terabytes of data. The Connector is now generally available.