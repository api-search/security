---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Aiven REST API
  slug: aiven-api
  spec_type: OpenAPI
  url: https://api.aiven.io/doc/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aiven.io
  spf: true
hosts:
- cert_expires: Oct  2 14:27:42 2026 GMT
  host: aiven.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 12:44:58 2026 GMT
  host: api.aiven.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aiven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aiven, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aiven
provider_slug: aiven
slug: aiven-domain-security
source_filename: aiven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiven.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:27:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aiven.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:44:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aiven.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiven/refs/heads/main/security/aiven-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Managed Data Infrastructure
- Apache Kafka
- PostgreSQL
- OpenSearch
- ClickHouse
- Redis
- MySQL
- Open Source
- Cloud Database
- DBaaS
- Data Streaming
- Data Platform
---
