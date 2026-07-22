---
api_specs:
- filename: tessell-openapi-original.json
  format: json
  label: Tessell API
  slug: tessell-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessell/refs/heads/main/openapi/tessell-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tessell.com
  spf: true
hosts:
- cert_expires: Oct 12 06:03:24 2026 GMT
  host: www.tessell.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: console.tessell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:27:07 2026 GMT
  host: developer.tessell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tessell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tessell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tessell
provider_slug: tessell
slug: tessell-domain-security
source_filename: tessell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tessell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 06:03:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.tessell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tessell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:27:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tessell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessell/refs/heads/main/security/tessell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Databases
- DBaaS
- Multi-Cloud
- Oracle
- PostgreSQL
- MySQL
- SQL Server
- Data Infrastructure
---
