---
api_specs:
- filename: openapi.json
  format: json
  label: KonbiniAPI Main Spec
  slug: main
  spec_type: OpenAPI
  url: https://docs.konbiniapi.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: konbiniapi.com
  spf: true
hosts:
- cert_expires: Oct  5 15:04:00 2026 GMT
  host: docs.konbiniapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:47:55 2026 GMT
  host: api.konbiniapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Konbiniapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KonbiniAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: KonbiniAPI
provider_slug: konbiniapi
slug: konbiniapi-domain-security
source_filename: konbiniapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.konbiniapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.konbiniapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:47:55 2026 GMT\n  hsts: null\ndomains:\n- domain: konbiniapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/security/konbiniapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- API
- Social Media
- Instagram
- TikTok
- ActivityStreams 2.0
- Scraping
- Data Extraction
- Public Data
- Influencer Marketing
- Social Listening
- Creator Tools
- MCP
- Model Context Protocol
---
