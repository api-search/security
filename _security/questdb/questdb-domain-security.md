---
api_specs:
- filename: questdb-openapi.yml
  format: yaml
  label: QuestDB HTTP REST API
  slug: rest-http
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/questdb/refs/heads/main/openapi/questdb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: questdb.com
  spf: true
hosts:
- cert_expires: Sep 10 21:13:54 2026 GMT
  host: questdb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Questdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuestDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QuestDB
provider_slug: questdb
slug: questdb-domain-security
source_filename: questdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: questdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:13:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: questdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/questdb/refs/heads/main/security/questdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Time-Series
- SQL
- Open Source
- Performance
- ILP
- PostgreSQL
---
