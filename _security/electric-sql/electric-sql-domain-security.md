---
api_specs:
- filename: electric-sql-http-sync-api-openapi.yml
  format: yaml
  label: Electric HTTP Sync API
  slug: http-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electric-sql/refs/heads/main/openapi/electric-sql-http-sync-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: electric.ax
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: electric-sql.cloud
  spf: true
hosts:
- cert_expires: Sep 25 08:34:53 2026 GMT
  host: electric.ax
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 13:18:02 2026 GMT
  host: api.electric-sql.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electric Sql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ElectricSQL, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ElectricSQL
provider_slug: electric-sql
slug: electric-sql-domain-security
source_filename: electric-sql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: electric.ax\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:34:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.electric-sql.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:18:02 2026 GMT\n  hsts: null\ndomains:\n- domain: electric.ax\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: electric-sql.cloud\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electric-sql/refs/heads/main/security/electric-sql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Database
- Sync
- Local-First
- Postgres
- Real-Time
- Open Source
---
