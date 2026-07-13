---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: confluent.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: confluent.cloud
  spf: true
hosts:
- cert_expires: Sep 15 09:44:59 2026 GMT
  host: www.confluent.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: docs.confluent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.confluent.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confluent The Data Streaming Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confluent | the Data Streaming Platform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Confluent | the Data Streaming Platform
provider_slug: confluent-the-data-streaming-platform
slug: confluent-the-data-streaming-platform-domain-security
source_filename: confluent-the-data-streaming-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.confluent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.confluent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: false\n- host: api.confluent.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: confluent.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: confluent.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/security/confluent-the-data-streaming-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache Flink
- Apache Kafka
- Confluent Cloud
- Connectors
- Data Streaming
- Event Streaming
- Kafka Connect
- ksqlDB
- Real-Time Data
- REST
- Schema Registry
- Stream Processing
---
