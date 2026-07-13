---
api_specs:
- filename: openapi.json
  format: json
  label: Val Town REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.val.town/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: val.town
  spf: true
hosts:
- cert_expires: Oct  7 04:41:21 2026 GMT
  host: www.val.town
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:39:40 2026 GMT
  host: docs.val.town
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 00:14:34 2026 GMT
  host: api.val.town
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Val Town Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Val Town, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Val Town
provider_slug: val-town
slug: val-town-domain-security
source_filename: val-town-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.val.town\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:41:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.val.town\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:39:40 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.val.town\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:14:34 2026 GMT\n  hsts: null\ndomains:\n- domain: val.town\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/security/val-town-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Developer Tools
- Serverless
- JavaScript
- TypeScript
- Social Coding
- HTTP Endpoints
- Cron Jobs
- Email
- SQLite
- Blob Storage
---
