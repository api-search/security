---
api_specs:
- filename: artie-openapi-original.yml
  format: yaml
  label: Artie API
  slug: artie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artie.com
  spf: true
hosts:
- cert_expires: Sep  8 07:06:51 2026 GMT
  host: www.artie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 03:38:33 2026 GMT
  host: api.artie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artie, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artie
provider_slug: artie
slug: artie-domain-security
source_filename: artie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:06:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.artie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:38:33 2026 GMT\n  hsts: null\ndomains:\n- domain: artie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/security/artie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Replication
- Change Data Capture
- Data Integration
- ETL
- Streaming
- Databases
- Data Warehouse
- CDC
- Data Engineering
---
