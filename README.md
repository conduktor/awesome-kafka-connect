# Awesome Kafka Connect

A curated list of Kafka Connect connectors, tools, and resources.

## Contents

- [Databases](#databases)
  - [Relational Databases (JDBC)](#relational-databases-jdbc)
  - [MongoDB](#mongodb)
  - [Cassandra](#cassandra)
  - [Neo4j](#neo4j)
  - [ClickHouse](#clickhouse)
  - [CockroachDB](#cockroachdb)
  - [SingleStore (MemSQL)](#singlestore-memsql)
  - [Couchbase](#couchbase)
  - [MarkLogic](#marklogic)
  - [ArangoDB](#arangodb)
  - [OrientDB](#orientdb)
  - [HBase](#hbase)
- [Change Data Capture (CDC)](#change-data-capture-cdc)
- [Cloud Storage](#cloud-storage)
  - [Amazon S3](#amazon-s3)
  - [Google Cloud Storage](#google-cloud-storage)
  - [Azure Blob Storage](#azure-blob-storage)
  - [MinIO](#minio)
- [Data Warehouses](#data-warehouses)
  - [Snowflake](#snowflake)
  - [BigQuery](#bigquery)
  - [Redshift](#redshift)
  - [Databricks](#databricks)
- [Open Table Formats (Lakehouse)](#open-table-formats-lakehouse)
  - [Apache Iceberg](#apache-iceberg)
  - [Apache Hudi](#apache-hudi)
  - [Delta Lake](#delta-lake)
- [Search Engines](#search-engines)
  - [Elasticsearch](#elasticsearch)
  - [OpenSearch](#opensearch)
  - [Solr](#solr)
  - [Algolia](#algolia)
- [Vector Databases](#vector-databases)
  - [Milvus](#milvus)
  - [Weaviate](#weaviate)
  - [Pinecone](#pinecone)
- [Time-Series Databases](#time-series-databases)
  - [InfluxDB](#influxdb)
  - [TimescaleDB](#timescaledb)
  - [QuestDB](#questdb)
  - [Prometheus](#prometheus)
- [Message Queues](#message-queues)
  - [IBM MQ](#ibm-mq)
  - [RabbitMQ](#rabbitmq)
  - [ActiveMQ](#activemq)
  - [JMS (Generic)](#jms-generic)
  - [MQTT](#mqtt)
  - [Amazon SQS](#amazon-sqs)
  - [Google Pub/Sub](#google-pubsub)
  - [Azure Event Hubs](#azure-event-hubs)
  - [Solace PubSub+](#solace-pubsub)
- [File Systems](#file-systems)
  - [FilePulse](#filepulse)
  - [SpoolDir](#spooldir)
  - [SFTP/FTP](#sftpftp)
  - [HDFS](#hdfs)
- [HTTP & REST](#http--rest)
- [Logging & Monitoring](#logging--monitoring)
  - [Splunk](#splunk)
  - [Datadog](#datadog)
  - [New Relic](#new-relic)
  - [PagerDuty](#pagerduty)
  - [Syslog](#syslog)
- [Caching](#caching)
  - [Redis](#redis)
  - [Hazelcast](#hazelcast)
- [CRM & Marketing](#crm--marketing)
  - [Salesforce](#salesforce)
  - [ServiceNow](#servicenow)
  - [Zendesk](#zendesk)
  - [Marketo](#marketo)
- [Enterprise Systems](#enterprise-systems)
  - [SAP](#sap)
  - [Oracle](#oracle)
- [Social Media](#social-media)
  - [Twitter](#twitter)
- [Email](#email)
- [IoT](#iot)
- [Blockchain](#blockchain)
- [Data Formats & Transformations](#data-formats--transformations)
- [Multi-Connector Packages](#multi-connector-packages)
  - [Lenses Stream Reactor](#lenses-stream-reactor)
  - [Aiven Open Source](#aiven-open-source)
- [Tools & Utilities](#tools--utilities)

---

## Databases

### Relational Databases (JDBC)

- [confluentinc/kafka-connect-jdbc](https://github.com/confluentinc/kafka-connect-jdbc) - Confluent's JDBC source and sink connector supporting MySQL, PostgreSQL, Oracle, SQL Server, DB2, SQLite, and more
- [Aiven-Open/jdbc-connector-for-apache-kafka](https://github.com/Aiven-Open/jdbc-connector-for-apache-kafka) - Aiven's JDBC sink and source connectors for Apache Kafka
- [Debezium JDBC Sink](https://debezium.io/documentation/reference/stable/connectors/jdbc.html) - Debezium's JDBC sink connector supporting multiple databases

### MongoDB

- [mongodb/mongo-kafka](https://github.com/mongodb/mongo-kafka) - Official MongoDB Kafka Connector (source and sink)
- [hpgrahsl/kafka-connect-mongodb](https://github.com/hpgrahsl/kafka-connect-mongodb) - Community MongoDB sink connector

### Cassandra

- [datastax/kafka-sink](https://github.com/datastax/kafka-sink) - DataStax Apache Kafka Connector for Apache Cassandra and DataStax Enterprise
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Includes Cassandra source and sink (part of Stream Reactor)

### Neo4j

- [neo4j-contrib/neo4j-streams](https://github.com/neo4j-contrib/neo4j-streams) - Neo4j Kafka Streams integration with Kafka Connect sink

### ClickHouse

- [ClickHouse/clickhouse-kafka-connect](https://github.com/ClickHouse/clickhouse-kafka-connect) - Official ClickHouse Kafka Connect sink connector

### CockroachDB

- Works with JDBC connector using PostgreSQL wire protocol

### SingleStore (MemSQL)

- [memsql/singlestore-kafka-connector](https://github.com/memsql/singlestore-kafka-connector) - Official SingleStore Kafka Connector

### Couchbase

- [couchbase/kafka-connect-couchbase](https://github.com/couchbase/kafka-connect-couchbase) - Official Couchbase Kafka Connector (source and sink)

### MarkLogic

- [marklogic-community/kafka-marklogic-connector](https://github.com/marklogic-community/kafka-marklogic-connector) - MarkLogic Kafka Connector

### ArangoDB

- [jaredpetersen/kafka-connect-arangodb](https://github.com/jaredpetersen/kafka-connect-arangodb) - Kafka Connect sink connector for ArangoDB

### OrientDB

- Community JDBC-based integrations available

### HBase

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Includes HBase sink connector

---

## Change Data Capture (CDC)

- [debezium/debezium](https://github.com/debezium/debezium) - Leading CDC platform with connectors for MySQL, PostgreSQL, MongoDB, Oracle, SQL Server, Db2, Cassandra, Vitess, Spanner
- [zendesk/maxwell](https://github.com/zendesk/maxwell) - Maxwell's daemon for MySQL CDC to Kafka
- [alibaba/canal](https://github.com/alibaba/canal) - Alibaba MySQL binlog incremental subscription & consumption
- [confluentinc/kafka-connect-jdbc](https://github.com/confluentinc/kafka-connect-jdbc) - Query-based CDC using incrementing/timestamp columns

---

## Cloud Storage

### Amazon S3

- [confluentinc/kafka-connect-storage-cloud](https://github.com/confluentinc/kafka-connect-storage-cloud) - Confluent's S3 sink connector
- [Aiven-Open/cloud-storage-connectors-for-apache-kafka](https://github.com/Aiven-Open/cloud-storage-connectors-for-apache-kafka) - Aiven's cloud storage connectors (S3, GCS, Azure)
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - AWS S3 source and sink connectors
- [spredfast/kafka-connect-s3](https://github.com/spredfast/kafka-connect-s3) - Spredfast S3 sink connector

### Google Cloud Storage

- [confluentinc/kafka-connect-storage-cloud](https://github.com/confluentinc/kafka-connect-storage-cloud) - Confluent's GCS sink connector
- [Aiven-Open/cloud-storage-connectors-for-apache-kafka](https://github.com/Aiven-Open/cloud-storage-connectors-for-apache-kafka) - Aiven's GCS connector
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - GCP Storage sink connector

### Azure Blob Storage

- [confluentinc/kafka-connect-storage-cloud](https://github.com/confluentinc/kafka-connect-storage-cloud) - Confluent's Azure Blob sink connector
- [Aiven-Open/cloud-storage-connectors-for-apache-kafka](https://github.com/Aiven-Open/cloud-storage-connectors-for-apache-kafka) - Aiven's Azure Blob connector
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Azure Data Lake sink connector

### MinIO

- Works with any S3-compatible connector

---

## Data Warehouses

### Snowflake

- [snowflakedb/snowflake-kafka-connector](https://github.com/snowflakedb/snowflake-kafka-connector) - Official Snowflake Kafka Connector

### BigQuery

- [Aiven-Open/bigquery-connector-for-apache-kafka](https://github.com/Aiven-Open/bigquery-connector-for-apache-kafka) - Aiven's BigQuery sink connector
- [wepay/kafka-connect-bigquery](https://github.com/wepay/kafka-connect-bigquery) - WePay BigQuery sink connector
- [confluentinc/kafka-connect-bigquery](https://www.confluent.io/hub/wepay/kafka-connect-bigquery) - Confluent Hub version

### Redshift

- [Aiven-Open/jdbc-connector-for-apache-kafka](https://github.com/Aiven-Open/jdbc-connector-for-apache-kafka) - Via JDBC
- Confluent Redshift sink connector (commercial)

### Databricks

- [databricks/databricks-sql-connector](https://github.com/databricks/databricks-sql-connector) - Databricks SQL connector
- Works with Delta Lake connector for direct lakehouse integration

---

## Open Table Formats (Lakehouse)

### Apache Iceberg

- [tabular-io/iceberg-kafka-connect](https://github.com/tabular-io/iceberg-kafka-connect) - Tabular's Iceberg Kafka Connect sink
- [getindata/kafka-connect-iceberg-sink](https://github.com/getindata/kafka-connect-iceberg-sink) - GetInData's Iceberg sink connector

### Apache Hudi

- [apache/hudi](https://github.com/apache/hudi) - Includes DeltaStreamer for Kafka ingestion
- [hudi-kafka-connect](https://hudi.apache.org/docs/kafka_connect) - Official Hudi Kafka Connect sink

### Delta Lake

- [delta-io/delta](https://github.com/delta-io/delta) - Delta Lake with Spark Streaming Kafka integration

---

## Search Engines

### Elasticsearch

- [confluentinc/kafka-connect-elasticsearch](https://github.com/confluentinc/kafka-connect-elasticsearch) - Confluent's Elasticsearch sink connector
- [Aiven-Open/elasticsearch-connector-for-apache-kafka](https://github.com/Aiven-Open/elasticsearch-connector-for-apache-kafka) - Aiven's Elasticsearch sink connector
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Elasticsearch sink connector

### OpenSearch

- [Aiven-Open/opensearch-connector-for-apache-kafka](https://github.com/Aiven-Open/opensearch-connector-for-apache-kafka) - Aiven's OpenSearch connector
- [dmathieu/kafka-connect-opensearch](https://github.com/dmathieu/kafka-connect-opensearch) - Community OpenSearch connector

### Solr

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Solr sink connector

### Algolia

- [algolia/algolia-sitemap-generator](https://github.com/algolia/algolia-sitemap-generator) - Indirect integration via indexing pipelines

---

## Vector Databases

### Milvus

- [zilliztech/kafka-connect-milvus](https://github.com/zilliztech/kafka-connect-milvus) - Milvus Kafka Connect sink connector

### Weaviate

- [weaviate/weaviate](https://github.com/weaviate/weaviate) - Kafka Connect integration available

### Pinecone

- Pinecone Kafka Connect sink connector (commercial)

---

## Time-Series Databases

### InfluxDB

- [influxdata/kafka-connect-influxdb](https://github.com/influxdata/kafka-connect-influxdb) - Official InfluxDB sink connector
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - InfluxDB sink connector

### TimescaleDB

- Works with PostgreSQL JDBC connector

### QuestDB

- [questdb/kafka-questdb-connector](https://github.com/questdb/kafka-questdb-connector) - Official QuestDB Kafka Connect sink

### Prometheus

- [riferrei/prometheus-kafka-connect](https://github.com/riferrei/prometheus-kafka-connect) - Prometheus metrics sink connector

---

## Message Queues

### IBM MQ

- [ibm-messaging/kafka-connect-mq-source](https://github.com/ibm-messaging/kafka-connect-mq-source) - Official IBM MQ source connector
- [ibm-messaging/kafka-connect-mq-sink](https://github.com/ibm-messaging/kafka-connect-mq-sink) - Official IBM MQ sink connector

### RabbitMQ

- [ibm-messaging/kafka-connect-rabbitmq-source](https://github.com/ibm-messaging/kafka-connect-rabbitmq-source) - IBM's RabbitMQ source connector
- Confluent RabbitMQ source connector (commercial)

### ActiveMQ

- [macronova/kafka-connect-jms](https://github.com/macronova/kafka-connect-jms) - JMS connector supporting ActiveMQ

### JMS (Generic)

- [macronova/kafka-connect-jms](https://github.com/macronova/kafka-connect-jms) - Generic JMS source and sink for IBM MQ, ActiveMQ, TIBCO EMS, Solace PubSub, RabbitMQ
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - JMS source connector

### MQTT

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - MQTT source connector
- Confluent MQTT source connector (commercial)
- [hivemq/hivemq-kafka-extension](https://github.com/hivemq/hivemq-kafka-extension) - HiveMQ Enterprise Kafka Extension

### Amazon SQS

- [nordstrom/kafka-connect-sqs](https://github.com/Nordstrom/kafka-connect-sqs) - Nordstrom's SQS source and sink connector
- Confluent SQS source/sink connectors (commercial)

### Google Pub/Sub

- [googleapis/java-pubsub-group-kafka-connector](https://github.com/googleapis/java-pubsub-group-kafka-connector) - Official Google Pub/Sub Kafka connector
- Confluent Pub/Sub connector (commercial)

### Azure Event Hubs

- Works natively via Kafka protocol support in Azure Event Hubs

### Solace PubSub+

- [SolaceProducts/pubsubplus-connector-kafka-source](https://github.com/SolaceProducts/pubsubplus-connector-kafka-source) - Solace PubSub+ source connector
- [SolaceProducts/pubsubplus-connector-kafka-sink](https://github.com/SolaceProducts/pubsubplus-connector-kafka-sink) - Solace PubSub+ sink connector

---

## File Systems

### FilePulse

- [streamthoughts/kafka-connect-file-pulse](https://github.com/streamthoughts/kafka-connect-file-pulse) - Multipurpose connector for CSV, JSON, XML, Avro files from local, S3, GCS, Azure

### SpoolDir

- [jcustenborder/kafka-connect-spooldir](https://github.com/jcustenborder/kafka-connect-spooldir) - Watch directories for CSV, JSON, binary files

### SFTP/FTP

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - FTP source connector
- [mglaserna/kafka-connect-sftp](https://github.com/mglaserna/kafka-connect-sftp) - SFTP sink connector
- Confluent SFTP source connector (commercial)

### HDFS

- [confluentinc/kafka-connect-hdfs](https://github.com/confluentinc/kafka-connect-hdfs) - Confluent's HDFS sink connector

---

## HTTP & REST

- [Aiven-Open/http-connector-for-apache-kafka](https://github.com/Aiven-Open/http-connector-for-apache-kafka) - Aiven's HTTP sink connector
- [llofberg/kafka-connect-rest](https://github.com/llofberg/kafka-connect-rest) - REST source and sink connector
- [asaintsever/kafka-connect-http-sink](https://github.com/asaintsever/kafka-connect-http-sink) - HTTP sink connector
- [thomaskwscott/kafka-connect-http](https://github.com/thomaskwscott/kafka-connect-http) - HTTP sink connector with regex transformations
- Confluent HTTP source and sink connectors (commercial)

---

## Logging & Monitoring

### Splunk

- [splunk/kafka-connect-splunk](https://github.com/splunk/kafka-connect-splunk) - Official Splunk sink connector

### Datadog

- [DataDog/datadog-kafka-connect](https://github.com/DataDog/datadog-kafka-connect-logs) - Datadog logs sink connector

### New Relic

- [newrelic/kafka-connect-newrelic](https://github.com/newrelic/kafka-connect-newrelic) - New Relic sink connector

### PagerDuty

- [pagerduty/kafka-connect-pagerduty](https://github.com/pagerduty/kafka-connect-pagerduty) - PagerDuty events sink connector

### Syslog

- [jcustenborder/kafka-connect-syslog](https://github.com/jcustenborder/kafka-connect-syslog) - Syslog source connector

---

## Caching

### Redis

- [jcustenborder/kafka-connect-redis](https://github.com/jcustenborder/kafka-connect-redis) - Redis sink connector
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Redis sink connector

### Hazelcast

- [hazelcast/hazelcast-jet-contrib](https://github.com/hazelcast/hazelcast-jet-contrib) - Hazelcast Jet connectors for Kafka

---

## CRM & Marketing

### Salesforce

- [jcustenborder/kafka-connect-salesforce](https://github.com/jcustenborder/kafka-connect-salesforce) - Salesforce streaming and push topics source
- Confluent Salesforce connectors (commercial)

### ServiceNow

- Confluent ServiceNow source connector (commercial)

### Zendesk

- Confluent Zendesk source connector (commercial)

### Marketo

- Confluent Marketo source connector (commercial)

---

## Enterprise Systems

### SAP

- SAP Kafka Connect adapters (commercial)

### Oracle

- Works with Debezium Oracle connector or JDBC connector

---

## Social Media

### Twitter

- [jcustenborder/kafka-connect-twitter](https://github.com/jcustenborder/kafka-connect-twitter) - Twitter streaming API source connector
- [Eneco/kafka-connect-twitter](https://github.com/Eneco/kafka-connect-twitter) - Twitter source and sink connector

---

## Email

- [jcustenborder/kafka-connect-email](https://github.com/jcustenborder/kafka-connect-email) - IMAP email source connector
- [wardziniak/kafka-connect-email](https://github.com/wardziniak/kafka-connect-email) - SMTP email sink connector
- [cloudstark/kafka-connect-sendgrid](https://github.com/cloudstark/kafka-connect-sendgrid) - SendGrid sink connector

---

## IoT

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - MQTT source connector for IoT devices
- [hivemq/hivemq-kafka-extension](https://github.com/hivemq/hivemq-kafka-extension) - MQTT broker to Kafka bridge

---

## Blockchain

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Blockchain source connector

---

## Data Formats & Transformations

- [Aiven-Open/transforms-for-apache-kafka-connect](https://github.com/Aiven-Open/transforms-for-apache-kafka-connect) - Aiven's collection of Single Message Transformations (SMTs)
- [jcustenborder/kafka-connect-transform-common](https://github.com/jcustenborder/kafka-connect-transform-common) - Common transformations library
- [confluentinc/connect-transforms](https://github.com/confluentinc/connect-transforms) - Confluent community SMTs

---

## Multi-Connector Packages

### Lenses Stream Reactor

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - 30+ connectors including AWS S3, Azure Data Lake, Cassandra, Elasticsearch, FTP, HBase, HDFS, HTTP, InfluxDB, JMS, Kudu, MongoDB, MQTT, Redis, Solr, and more

### Aiven Open Source

- [Aiven-Open](https://github.com/Aiven-Open) - Open source connectors for BigQuery, cloud storage (S3/GCS/Azure), Elasticsearch, HTTP, JDBC, OpenSearch, plus SMTs and Kafka tools

---

## Tools & Utilities

- [Conduktor Console](https://conduktor.io) - Complete Kafka Connect management UI
- [kafka-connect-ui](https://github.com/lensesio/kafka-connect-ui) - Lenses Kafka Connect UI
- [Kafdrop](https://github.com/obsidiandynamics/kafdrop) - Kafka web UI with Connect support
- [akhq](https://github.com/tchiotludo/akhq) - Kafka HQ with Kafka Connect management
- [strimzi/strimzi-kafka-operator](https://github.com/strimzi/strimzi-kafka-operator) - Kubernetes operator with Kafka Connect support
- [confluentinc/kafka-connect-datagen](https://github.com/confluentinc/kafka-connect-datagen) - Generate sample data for testing

---

## Contributing

Contributions welcome! Please read the contribution guidelines first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
