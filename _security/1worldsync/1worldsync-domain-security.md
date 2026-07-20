---
api_specs:
- filename: 1worldsync-content1-openapi-original.json
  format: json
  label: 1WorldSync Content1 API
  slug: 1worldsync-content1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1worldsync/refs/heads/main/openapi/1worldsync-content1-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 1worldsync.com
  spf: true
hosts:
- cert_expires: Sep 29 06:09:50 2026 GMT
  host: 1worldsync.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 22:15:25 2026 GMT
  host: developer.1worldsync.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 14:11:33 2026 GMT
  host: content1-api.1worldsync.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Worldsync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1WorldSync, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 1WorldSync
provider_slug: 1worldsync
slug: 1worldsync-domain-security
source_filename: 1worldsync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1worldsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:09:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.1worldsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:15:25 2026 GMT\n  hsts: false\n- host: content1-api.1worldsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 14:11:33 2026 GMT\n  hsts: false\ndomains:\n- domain: 1worldsync.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1worldsync/refs/heads/main/security/1worldsync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Product Content
- GDSN
- Data Syndication
- Master Data
- Digital Shelf
- Product Information Management
- PIM
- CPG
- Retail
- GS1
---
