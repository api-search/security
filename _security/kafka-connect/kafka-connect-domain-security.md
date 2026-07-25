---
api_specs:
- filename: kafka-connect-connector-plugins-api-openapi.yml
  format: yaml
  label: Kafka Connect Connector Plugins API
  slug: kafka-connect-connector-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kafka-connect/refs/heads/main/openapi/kafka-connect-connector-plugins-api-openapi.yml
- filename: kafka-connect-connectors-api-openapi.yml
  format: yaml
  label: Kafka Connect Connectors API
  slug: kafka-connect-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kafka-connect/refs/heads/main/openapi/kafka-connect-connectors-api-openapi.yml
- filename: kafka-connect-kafka-connect-rest-api-api-openapi.yml
  format: yaml
  label: Kafka Connect Kafka Connect REST API API
  slug: kafka-connect-kafka-connect-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kafka-connect/refs/heads/main/openapi/kafka-connect-kafka-connect-rest-api-api-openapi.yml
description: ''
domains:
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
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: kafka.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kafka Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kafka Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kafka Connect
provider_slug: kafka-connect
slug: kafka-connect-domain-security
source_filename: kafka-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kafka.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kafka-connect/refs/heads/main/security/kafka-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache Kafka
- Connectors
- Data Integration
- ETL
- Streaming
---
