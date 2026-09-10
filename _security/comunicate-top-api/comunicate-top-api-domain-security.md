---
api_specs:
- filename: openapi.json
  format: json
  label: Comunicate.top API
  slug: comunicatetop-api
  spec_type: OpenAPI
  url: https://comunicate.top/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: comunicate.top
  spf: true
hosts:
- cert_expires: Nov 16 13:16:24 2026 GMT
  host: comunicate.top
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 13:16:24 2026 GMT
  host: app.comunicate.top
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Comunicate Top Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comunicate.top API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Comunicate.top API
provider_slug: comunicate-top-api
slug: comunicate-top-api-domain-security
source_filename: comunicate-top-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comunicate.top\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 13:16:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.comunicate.top\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 13:16:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: comunicate.top\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/security/comunicate-top-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Press Releases
- Advertorials
- PR
- Publishing
- Media
- SEO
- Link Building
- Content Marketing
- Romania
- MCP
- Open Data
- Webhooks
- OAuth
---
