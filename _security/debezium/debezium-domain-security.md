---
api_specs:
- filename: debezium-connect.yml
  format: yaml
  label: Debezium Kafka Connect REST API
  slug: debezium-kafka-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debezium/refs/heads/main/openapi/debezium-connect.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: debezium.io
  spf: true
hosts:
- cert_expires: Sep 20 08:15:45 2026 GMT
  host: debezium.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Debezium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Debezium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Debezium
provider_slug: debezium
slug: debezium-domain-security
source_filename: debezium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: debezium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:15:45 2026 GMT\n  hsts: false\ndomains:\n- domain: debezium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debezium/refs/heads/main/security/debezium-domain-security.yml
summary_line: TLSv1.3
tags:
- Apache Kafka
- CDC
- Change Data Capture
- Databases
- Event Streaming
- Open Source
---
