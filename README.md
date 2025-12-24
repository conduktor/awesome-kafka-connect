# Awesome Kafka Connect

A curated list of Kafka Connect connectors.

> See also: [awesome-kafka](https://github.com/conduktor/awesome-kafka) - A comprehensive list of Apache Kafka resources, tools, and libraries

## Contents

- [Databases](#databases)
  - [Relational Databases (JDBC)](#relational-databases-jdbc)
  - [MongoDB](#mongodb)
  - [Cassandra](#cassandra)
  - [Neo4j](#neo4j)
  - [TigerGraph](#tigergraph)
  - [JanusGraph](#janusgraph)
  - [ClickHouse](#clickhouse)
  - [CockroachDB](#cockroachdb)
  - [SingleStore (MemSQL)](#singlestore-memsql)
  - [Couchbase](#couchbase)
  - [CouchDB](#couchdb)
  - [Azure Cosmos DB](#azure-cosmos-db)
  - [MarkLogic](#marklogic)
  - [ScyllaDB](#scylladb)
  - [ArangoDB](#arangodb)
  - [OrientDB](#orientdb)
  - [HBase](#hbase)
  - [DynamoDB](#dynamodb)
  - [YugabyteDB](#yugabytedb)
  - [Apache Kudu](#apache-kudu)
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
  - [Azure Data Explorer (Kusto)](#azure-data-explorer-kusto)
  - [Apache Pinot](#apache-pinot)
  - [Apache Druid](#apache-druid)
  - [StarRocks](#starrocks)
  - [Apache Doris](#apache-doris)
  - [Databend](#databend)
  - [Teradata](#teradata)
  - [Vertica](#vertica)
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
  - [Qdrant](#qdrant)
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
  - [Amazon Kinesis](#amazon-kinesis)
  - [Amazon EventBridge](#amazon-eventbridge)
  - [NATS](#nats)
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
  - [Grafana Loki](#grafana-loki)
  - [OpenTelemetry](#opentelemetry)
- [Caching](#caching)
  - [Redis](#redis)
  - [Hazelcast](#hazelcast)
  - [Apache Geode](#apache-geode)
  - [Memcached](#memcached)
  - [Apache Ignite](#apache-ignite)
- [CRM & Marketing](#crm--marketing)
  - [Salesforce](#salesforce)
  - [ServiceNow](#servicenow)
  - [Zendesk](#zendesk)
  - [Marketo](#marketo)
- [Developer Tools](#developer-tools)
  - [GitLab](#gitlab)
  - [GitHub](#github)
  - [Jira](#jira)
- [Enterprise Systems](#enterprise-systems)
  - [SAP](#sap)
  - [Oracle](#oracle)
- [Social Media](#social-media)
  - [Slack](#slack)
  - [Telegram](#telegram)
  - [Twitter](#twitter)
- [Email](#email)
- [IoT](#iot)
- [Blockchain](#blockchain)
- [Data Formats & Transformations](#data-formats--transformations)
- [Data Generators & Testing](#data-generators--testing)
- [Real-Time Data Platforms](#real-time-data-platforms)
  - [Diffusion](#diffusion)
  - [Kafka-to-Kafka Replication](#kafka-to-kafka-replication)
- [Healthcare (HL7/FHIR)](#healthcare-hl7fhir)
- [GIS & Geospatial](#gis--geospatial)
- [Machine Learning & Feature Stores](#machine-learning--feature-stores)
- [Data Catalogs](#data-catalogs)
- [Multi-Connector Packages](#multi-connector-packages)
  - [Lenses Stream Reactor](#lenses-stream-reactor)
  - [Aiven Open Source](#aiven-open-source)
  - [Apache Camel](#apache-camel)
  - [Camunda Zeebe](#camunda-zeebe)
  - [Redpanda Connect](#redpanda-connect)

---

## Databases

### Relational Databases (JDBC)

- [confluentinc/kafka-connect-jdbc](https://github.com/confluentinc/kafka-connect-jdbc) - Confluent's JDBC source and sink connector supporting MySQL, PostgreSQL, Oracle, SQL Server, DB2, SQLite, and more
- [Aiven-Open/jdbc-connector-for-apache-kafka](https://github.com/Aiven-Open/jdbc-connector-for-apache-kafka) - Aiven's JDBC sink and source connectors for Apache Kafka
- [Debezium JDBC Sink](https://debezium.io/documentation/reference/stable/connectors/jdbc.html) - Debezium's JDBC sink connector supporting multiple databases

### MongoDB

- [mongodb/mongo-kafka](https://github.com/mongodb/mongo-kafka) - Official MongoDB Kafka Connector (source and sink)
- [hpgrahsl/kafka-connect-mongodb](https://github.com/hpgrahsl/kafka-connect-mongodb) - Community MongoDB sink connector
- [DataReply/kafka-connect-mongodb](https://github.com/DataReply/kafka-connect-mongodb) - MongoDB source and sink using oplog
- [teambition/kafka-connect-mongo](https://github.com/teambition/kafka-connect-mongo) - MongoDB source with Schema Registry support (archived)

### Cassandra

- [datastax/kafka-sink](https://github.com/datastax/kafka-sink) - DataStax Apache Kafka Connector for Apache Cassandra and DataStax Enterprise
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Includes Cassandra source and sink (part of Stream Reactor)

### Neo4j

- [neo4j-contrib/neo4j-streams](https://github.com/neo4j-contrib/neo4j-streams) - Neo4j Kafka Streams integration with Kafka Connect sink

### TigerGraph

- [tigergraph/ecosys](https://github.com/tigergraph/ecosys) - TigerGraph Kafka Connect connector (in tools/etl/tg-kafka-connect)

### JanusGraph

- [rayokota/janusgraph-kafka](https://github.com/rayokota/janusgraph-kafka) - Kafka storage adapter for JanusGraph graph database

### ClickHouse

- [ClickHouse/clickhouse-kafka-connect](https://github.com/ClickHouse/clickhouse-kafka-connect) - Official ClickHouse Kafka Connect sink connector

### CockroachDB

- Works with JDBC connector using PostgreSQL wire protocol

### SingleStore (MemSQL)

- [memsql/singlestore-kafka-connector](https://github.com/memsql/singlestore-kafka-connector) - Official SingleStore Kafka Connector

### Couchbase

- [couchbase/kafka-connect-couchbase](https://github.com/couchbase/kafka-connect-couchbase) - Official Couchbase Kafka Connector (source and sink)

### CouchDB

- [xebia/kafka-connect-couchdb](https://github.com/xebia/kafka-connect-couchdb) - CouchDB / IBM Cloudant sink connector

### Azure Cosmos DB

- [microsoft/kafka-connect-cosmosdb](https://github.com/microsoft/kafka-connect-cosmosdb) - Azure Cosmos DB sink connector for SQL API

### MarkLogic

- [marklogic-community/kafka-marklogic-connector](https://github.com/marklogic-community/kafka-marklogic-connector) - MarkLogic Kafka Connector

### ScyllaDB

- [scylladb/kafka-connect-scylladb](https://github.com/scylladb/kafka-connect-scylladb) - Scylla-optimized sink connector

### Aerospike

- [jcustenborder/kafka-connect-aerospike](https://github.com/jcustenborder/kafka-connect-aerospike) - Aerospike source and sink connector

### ArangoDB

- [jaredpetersen/kafka-connect-arangodb](https://github.com/jaredpetersen/kafka-connect-arangodb) - Kafka Connect sink connector for ArangoDB

### OrientDB

- Community JDBC-based integrations available

### HBase

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Includes HBase sink connector

### DynamoDB

- [Confluent DynamoDB Sink](https://www.confluent.io/hub/confluentinc/kafka-connect-dynamodb) - Confluent DynamoDB sink connector (commercial)
- [trustpilot/kafka-connect-dynamodb](https://github.com/trustpilot/kafka-connect-dynamodb) - Open source DynamoDB sink connector

### YugabyteDB

- [yugabyte/yb-kafka-connector](https://github.com/yugabyte/yb-kafka-connector) - YugabyteDB Kafka Connect sink connector
- [yugabyte/debezium-connector-yugabytedb](https://github.com/yugabyte/debezium-connector-yugabytedb) - Debezium CDC source connector for YugabyteDB

### Apache Kudu

- [onfocusio/kafka-connect-kudu](https://github.com/onfocusio/kafka-connect-kudu) - Apache Kudu sink connector
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Kudu sink connector (part of Stream Reactor)

---

## Change Data Capture (CDC)

- [debezium/debezium](https://github.com/debezium/debezium) - Leading CDC platform with connectors for MySQL, PostgreSQL, MongoDB, Oracle, SQL Server, Db2, Cassandra, Vitess, Spanner
- [zendesk/maxwell](https://github.com/zendesk/maxwell) - Maxwell's daemon for MySQL CDC to Kafka
- [alibaba/canal](https://github.com/alibaba/canal) - Alibaba MySQL binlog incremental subscription & consumption
- [confluentinc/kafka-connect-jdbc](https://github.com/confluentinc/kafka-connect-jdbc) - Query-based CDC using incrementing/timestamp columns
- [thake/logminer-kafka-connect](https://github.com/thake/logminer-kafka-connect) - Oracle CDC using LogMiner (no GoldenGate required)

---

## Cloud Storage

### Amazon S3

- [confluentinc/kafka-connect-storage-cloud](https://github.com/confluentinc/kafka-connect-storage-cloud) - Confluent's S3 sink connector
- [Aiven-Open/cloud-storage-connectors-for-apache-kafka](https://github.com/Aiven-Open/cloud-storage-connectors-for-apache-kafka) - Aiven's cloud storage connectors (S3, GCS, Azure)
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - AWS S3 source and sink connectors
- [spredfast/kafka-connect-s3](https://github.com/spredfast/kafka-connect-s3) - Spredfast S3 sink connector
- [wix-incubator/kafka-connect-s3](https://github.com/wix-incubator/kafka-connect-s3) - S3 sink with block-GZIP compression and index files

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
- [nodefluent/bigquery-kafka-connect](https://github.com/nodefluent/bigquery-kafka-connect) - Node.js BigQuery source and sink connector

### Redshift

- [Aiven-Open/jdbc-connector-for-apache-kafka](https://github.com/Aiven-Open/jdbc-connector-for-apache-kafka) - Via JDBC
- Confluent Redshift sink connector (commercial)

### Databricks

- [databricks/databricks-sql-connector](https://github.com/databricks/databricks-sql-connector) - Databricks SQL connector
- Works with Delta Lake connector for direct lakehouse integration

### Azure Data Explorer (Kusto)

- [Azure/kafka-sink-azure-kusto](https://github.com/Azure/kafka-sink-azure-kusto) - Azure Data Explorer sink connector

### Apache Pinot

- [mhomaid/kafka-connect-apache-pinot](https://github.com/mhomaid/kafka-connect-apache-pinot) - Community sink connector for Apache Pinot

### Apache Druid

- [gianm/kafka-connect-druid](https://github.com/gianm/kafka-connect-druid) - Early-stage Apache Druid sink connector

### StarRocks

- [StarRocks/starrocks-connector-for-kafka](https://github.com/StarRocks/starrocks-connector-for-kafka) - Official StarRocks Kafka Connect sink connector

### Apache Doris

- [apache/doris-kafka-connector](https://github.com/apache/doris-kafka-connector) - Official Apache Doris Kafka Connect sink connector

### Databend

- [databendcloud/databend-kafka-connect](https://github.com/databendcloud/databend-kafka-connect) - Databend Kafka Connect sink connector

### Teradata

- Confluent Teradata connector (commercial) - JDBC-based source and sink

### Vertica

- Confluent Vertica connector (commercial)

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
- [jcustenborder/kafka-connect-solr](https://github.com/jcustenborder/kafka-connect-solr) - Solr sink connector with schemaless and cloud mode support

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

### Qdrant

- [qdrant/qdrant-kafka](https://github.com/qdrant/qdrant-kafka) - Qdrant vector database sink connector

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
- [jcustenborder/kafka-connect-rabbitmq](https://github.com/jcustenborder/kafka-connect-rabbitmq) - RabbitMQ source and sink connector
- Confluent RabbitMQ source connector (commercial)

### ActiveMQ

- [macronova/kafka-connect-jms](https://github.com/macronova/kafka-connect-jms) - JMS connector supporting ActiveMQ

### JMS (Generic)

- [macronova/kafka-connect-jms](https://github.com/macronova/kafka-connect-jms) - Generic JMS source and sink for IBM MQ, ActiveMQ, TIBCO EMS, Solace PubSub, RabbitMQ
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - JMS source connector

### MQTT

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - MQTT source connector
- [evokly/kafka-connect-mqtt](https://github.com/evokly/kafka-connect-mqtt) - MQTT source connector using Eclipse Paho
- Confluent MQTT source connector (commercial)
- [hivemq/hivemq-kafka-extension](https://github.com/hivemq/hivemq-kafka-extension) - HiveMQ Enterprise Kafka Extension

### Amazon SQS

- [nordstrom/kafka-connect-sqs](https://github.com/Nordstrom/kafka-connect-sqs) - Nordstrom's SQS source and sink connector
- Confluent SQS source/sink connectors (commercial)

### Amazon Kinesis

- [awslabs/kinesis-kafka-connector](https://github.com/awslabs/kinesis-kafka-connector) - Sink connector for Kinesis Data Streams and Firehose

### NATS

- [oystparis/kafka-connect-nats](https://github.com/oystparis/kafka-connect-nats) - NATS source and sink connector

### Amazon EventBridge

- [aws/eventbridge-kafka-connector](https://github.com/aws/eventbridge-kafka-connector) - Sink connector for Amazon EventBridge with S3 offloading

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
- [mmolimar/kafka-connect-fs](https://github.com/mmolimar/kafka-connect-fs) - FileSystem connector for local, HDFS, FTP, S3, GCS, Azure

### SFTP/FTP

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - FTP source connector
- [mglaserna/kafka-connect-sftp](https://github.com/mglaserna/kafka-connect-sftp) - SFTP sink connector
- Confluent SFTP source connector (commercial)

### HDFS

- [confluentinc/kafka-connect-hdfs](https://github.com/confluentinc/kafka-connect-hdfs) - Confluent's HDFS sink connector

---

## HTTP & REST

- [Aiven-Open/http-connector-for-apache-kafka](https://github.com/Aiven-Open/http-connector-for-apache-kafka) - Aiven's HTTP sink connector
- [castorm/kafka-connect-http](https://github.com/castorm/kafka-connect-http) - HTTP source for Change Data Capture from JSON APIs
- [llofberg/kafka-connect-rest](https://github.com/llofberg/kafka-connect-rest) - REST source and sink connector
- [asaintsever/kafka-connect-http-sink](https://github.com/asaintsever/kafka-connect-http-sink) - HTTP sink connector
- [thomaskwscott/kafka-connect-http](https://github.com/thomaskwscott/kafka-connect-http) - HTTP sink connector with regex transformations
- [axual/http-sink-connector](https://gitlab.com/axual/public/connect-plugins/http-sink-connector) - Axual HTTP sink connector (GitLab)
- [Platformatory/webhook-source-connector](https://github.com/Platformatory/webhook-source-connector) - Webhook source connector with Netty HTTP server
- [jcustenborder/kafka-connect-servlet](https://github.com/jcustenborder/kafka-connect-servlet) - Framework for building webhook-based connectors with embedded Jetty
- [jcustenborder/kafka-connect-github-webhook](https://github.com/jcustenborder/kafka-connect-github-webhook) - GitHub webhook source connector
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

### Grafana Loki

- [jeschkies/kafka-connect-loki](https://github.com/jeschkies/kafka-connect-loki) - Loki sink connector for log aggregation

### OpenTelemetry

- [conduktor/kafka-connect-opentelemetry](https://github.com/conduktor/kafka-connect-opentelemetry) - Source connector ingesting OTLP traces/metrics/logs into Kafka

---

## Caching

### Redis

- [jcustenborder/kafka-connect-redis](https://github.com/jcustenborder/kafka-connect-redis) - Redis sink connector
- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Redis sink connector

### Hazelcast

- [hazelcast/hazelcast-jet-contrib](https://github.com/hazelcast/hazelcast-jet-contrib) - Hazelcast Jet connectors for Kafka

### Apache Geode

- [apache/geode-kafka-connector](https://github.com/apache/geode-kafka-connector) - Apache Geode sink and source connector

### Memcached

- [jcustenborder/kafka-connect-memcached](https://github.com/jcustenborder/kafka-connect-memcached) - Memcached sink connector

### Apache Ignite

- Apache Ignite includes IgniteSinkConnector for streaming data from Kafka to Ignite caches

---

## CRM & Marketing

### Salesforce

- [jcustenborder/kafka-connect-salesforce](https://github.com/jcustenborder/kafka-connect-salesforce) - Salesforce streaming and push topics source
- [nodefluent/salesforce-kafka-connect](https://github.com/nodefluent/salesforce-kafka-connect) - Node.js Salesforce source and sink connector
- Confluent Salesforce connectors (commercial)

### ServiceNow

- Confluent ServiceNow source connector (commercial)

### Zendesk

- Confluent Zendesk source connector (commercial)

### Marketo

- Confluent Marketo source connector (commercial)

---

## Developer Tools

### GitLab

- [sami12rom/kafka-connect-gitlab](https://github.com/sami12rom/kafka-connect-gitlab) - GitLab source connector built with Kotlin

### GitHub

- [simplesteph/kafka-connect-github-source](https://github.com/simplesteph/kafka-connect-github-source) - GitHub events source connector

### Jira

- [algru/kafka-jira-source-connector](https://github.com/algru/kafka-jira-source-connector) - Jira REST API source connector

---

## Enterprise Systems

### SAP

- [SAP/kafka-connect-sap](https://github.com/SAP/kafka-connect-sap) - Official SAP HANA source and sink connector
- [santi81/kafka-connect-hana](https://github.com/santi81/kafka-connect-hana) - Alternative SAP HANA source and sink connector

### Oracle

- Works with Debezium Oracle connector or JDBC connector

---

## Social Media

### Slack

- [Mongey/kafka-connect-slack](https://github.com/Mongey/kafka-connect-slack) - Slack sink connector for posting messages

### Telegram

- [fbascheper/kafka-connect-telegram](https://github.com/fbascheper/kafka-connect-telegram) - Telegram source and sink connector

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
- [jcustenborder/kafka-connect-snmp](https://github.com/jcustenborder/kafka-connect-snmp) - SNMP trap source connector for network device monitoring

---

## Blockchain

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - Blockchain source connector

---

## Data Formats & Transformations

- [Aiven-Open/transforms-for-apache-kafka-connect](https://github.com/Aiven-Open/transforms-for-apache-kafka-connect) - Aiven's collection of Single Message Transformations (SMTs)
- [jcustenborder/kafka-connect-transform-common](https://github.com/jcustenborder/kafka-connect-transform-common) - Common transformations library
- [jcustenborder/kafka-connect-transform-maxmind](https://github.com/jcustenborder/kafka-connect-transform-maxmind) - MaxMind GeoIP2 transform to enrich records with geolocation data
- [jcustenborder/kafka-connect-transform-archive](https://github.com/jcustenborder/kafka-connect-transform-archive) - Transform to assist with archiving records to S3
- [jcustenborder/kafka-connect-transform-xml](https://github.com/jcustenborder/kafka-connect-transform-xml) - Transform for converting XML data to structured data
- [jcustenborder/kafka-connect-transform-fix](https://github.com/jcustenborder/kafka-connect-transform-fix) - Transform for reading FIX protocol messages
- [jcustenborder/kafka-connect-opentsdb](https://github.com/jcustenborder/kafka-connect-opentsdb) - Transform for parsing OpenTSDB wire format and telnet API protocol
- [confluentinc/connect-transforms](https://github.com/confluentinc/connect-transforms) - Confluent community SMTs

---

## Data Generators & Testing

- [confluentinc/kafka-connect-datagen](https://github.com/confluentinc/kafka-connect-datagen) - Confluent's datagen source connector for generating mock data with Avro schemas, JSON, or Protobuf
- [MichaelDrogalis/voluble](https://github.com/MichaelDrogalis/voluble) - Intelligent data generator with cross-topic relationships, tombstoning, and configurable rates
- [awslabs/amazon-msk-data-generator](https://github.com/awslabs/amazon-msk-data-generator) - AWS MSK data generator (Java port of Voluble) with referential consistency
- [sasakitoa/kafka-connect-random](https://github.com/sasakitoa/kafka-connect-random) - Simple random value source connector
- [simplesteph/kafka-connect-github-source](https://github.com/simplesteph/kafka-connect-github-source) - GitHub issues and pull requests source connector
- [conduktor/kafka-connect-wikimedia](https://github.com/conduktor/kafka-connect-wikimedia) - Wikimedia recent changes stream source connector

---

## Real-Time Data Platforms

### Diffusion

- [pushtechnology/diffusion-kafka-connect](https://github.com/pushtechnology/diffusion-kafka-connect) - Push Technology Diffusion source and sink for real-time streaming to web, mobile, and IoT edge clients

### Kafka-to-Kafka Replication

- [axual/kafka-synchronisation-connectors](https://gitlab.com/axual/public/connect-plugins/kafka-synchronisation-connectors) - Source and sink connectors for cross-cluster Kafka replication (GitLab)
- [kakao/kafka-sink-connector](https://github.com/kakao/kafka-sink-connector) - Kafka-to-Kafka sink with JsonPath filtering and sampling

---

## Healthcare (HL7/FHIR)

- [jcustenborder/kafka-connect-transform-hl7](https://github.com/jcustenborder/kafka-connect-transform-hl7) - Transform for reading HL7 healthcare message structures
- [UMEssen/Volcano-HL7-MLLP-Connector](https://github.com/UMEssen) - High-performance HL7 v2 MLLP listener to Kafka (Scala)
- Apache Camel FHIR Kafka Connector via camel-kafka-connector

---

## GIS & Geospatial

- [planetfederal/kafka-geoserver-plugin](https://github.com/planetfederal/kafka-geoserver-plugin) - GeoServer plugin sending WFS-T transactions to Kafka
- [52North/postgis-kafka-cdc](https://github.com/52North/postgis-kafka-cdc) - PostGIS CDC with Debezium (experimental)
- Debezium PostgreSQL connector supports PostGIS data types natively

---

## Machine Learning & Feature Stores

- [dwarszawski/kafka-connect-mlflow](https://github.com/dwarszawski/kafka-connect-mlflow) - MLflow Model Registry change tracking source connector
- Feast (Feature Store) integrates with Kafka for real-time feature ingestion

---

## Data Catalogs

- [jhollandus/kafka-atlas](https://github.com/jhollandus/kafka-atlas) - POC for integrating Kafka Connect and Schema Registry with Apache Atlas
- DataHub ingests Kafka Connect metadata for lineage tracking

---

## Multi-Connector Packages

### Lenses Stream Reactor

- [lensesio/stream-reactor](https://github.com/lensesio/stream-reactor) - 30+ connectors including AWS S3, Azure Data Lake, Cassandra, Elasticsearch, FTP, HBase, HDFS, HTTP, InfluxDB, JMS, Kudu, MongoDB, MQTT, Redis, Solr, and more

### Aiven Open Source

- [Aiven-Open](https://github.com/Aiven-Open) - Open source connectors for BigQuery, cloud storage (S3/GCS/Azure), Elasticsearch, HTTP, JDBC, OpenSearch, plus SMTs and Kafka tools

### Apache Camel

- [apache/camel-kafka-connector](https://github.com/apache/camel-kafka-connector) - 350+ connectors built on Apache Camel components, supporting AWS, Azure, GCP, databases, messaging systems, social media, and more

### Camunda Zeebe

- [camunda-community-hub/kafka-connect-zeebe](https://github.com/camunda-community-hub/kafka-connect-zeebe) - Zeebe source and sink connectors for workflow automation with Camunda

### Redpanda Connect

- [redpanda-data/connect](https://github.com/redpanda-data/connect) - Benthos-based declarative connectors for 200+ sources/sinks (Kafka compatible)

---

## Contributing

Contributions welcome! Please read the contribution guidelines first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
