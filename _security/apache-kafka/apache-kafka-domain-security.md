---
api_specs:
- filename: kafka-messaging.yml
  format: yaml
  label: Apache Kafka Messaging API
  slug: kafka-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/asyncapi/kafka-messaging.yml
- filename: apache-kafka-acl-api-openapi.yml
  format: yaml
  label: Apache Kafka ACL API
  slug: apache-kafka-acl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-acl-api-openapi.yml
- filename: apache-kafka-broker-api-openapi.yml
  format: yaml
  label: Apache Kafka Broker API
  slug: apache-kafka-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-broker-api-openapi.yml
- filename: apache-kafka-cluster-api-openapi.yml
  format: yaml
  label: Apache Kafka Cluster API
  slug: apache-kafka-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-cluster-api-openapi.yml
- filename: apache-kafka-connectors-api-openapi.yml
  format: yaml
  label: Apache Kafka Connectors API
  slug: apache-kafka-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-connectors-api-openapi.yml
- filename: apache-kafka-consumer-group-api-openapi.yml
  format: yaml
  label: Apache Kafka Consumer Group API
  slug: apache-kafka-consumer-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-consumer-group-api-openapi.yml
- filename: apache-kafka-offsets-api-openapi.yml
  format: yaml
  label: Apache Kafka Offsets API
  slug: apache-kafka-offsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-offsets-api-openapi.yml
- filename: apache-kafka-partition-api-openapi.yml
  format: yaml
  label: Apache Kafka Partition API
  slug: apache-kafka-partition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-partition-api-openapi.yml
- filename: apache-kafka-plugins-api-openapi.yml
  format: yaml
  label: Apache Kafka Plugins API
  slug: apache-kafka-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-plugins-api-openapi.yml
- filename: apache-kafka-records-api-openapi.yml
  format: yaml
  label: Apache Kafka Records API
  slug: apache-kafka-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-records-api-openapi.yml
- filename: apache-kafka-tasks-api-openapi.yml
  format: yaml
  label: Apache Kafka Tasks API
  slug: apache-kafka-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-tasks-api-openapi.yml
- filename: apache-kafka-topic-api-openapi.yml
  format: yaml
  label: Apache Kafka Topic API
  slug: apache-kafka-topic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/openapi/apache-kafka-topic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: confluent.io
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: docs.confluent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: kafka.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Kafka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Kafka, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apache Kafka
provider_slug: apache-kafka
slug: apache-kafka-domain-security
source_filename: apache-kafka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.confluent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: false\n- host: kafka.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: confluent.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/security/apache-kafka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open-Source
- Pub-Sub
---
