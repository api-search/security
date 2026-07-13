---
api_specs:
- filename: openapi.json
  format: json
  label: Xata Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://api.xata.tech/openapi.json
- filename: openapi.json
  format: json
  label: Xata SQL Gateway
  slug: sql-gateway
  spec_type: OpenAPI
  url: https://api.xata.tech/openapi.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xata.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: xata.tech
  spf: false
hosts:
- cert_expires: Sep  8 16:55:05 2026 GMT
  host: xata.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 06:40:25 2026 GMT
  host: api.xata.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xata, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xata
provider_slug: xata
slug: xata-domain-security
source_filename: xata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:55:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.xata.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:40:25 2026 GMT\n  hsts: null\ndomains:\n- domain: xata.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: xata.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xata/refs/heads/main/security/xata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Postgres
- Serverless
- Developer Tools
- Branching
- AI Agent
---
