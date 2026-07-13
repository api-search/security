---
api_specs:
- filename: the-index-fyi-openapi.yml
  format: yaml
  label: The Index Public API
  slug: indexes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-index-fyi/refs/heads/main/openapi/the-index-fyi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theindex.fyi
  spf: false
hosts:
- cert_expires: Aug  7 13:27:01 2026 GMT
  host: theindex.fyi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Index Fyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Index, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: The Index
provider_slug: the-index-fyi
slug: the-index-fyi-domain-security
source_filename: the-index-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theindex.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 13:27:01 2026 GMT\n  hsts: false\ndomains:\n- domain: theindex.fyi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-index-fyi/refs/heads/main/security/the-index-fyi-domain-security.yml
summary_line: TLSv1.3
tags:
- Indie Web
- Small Web
- Directories
- Search
- RSS
- Webrings
- Open Data
- JSON:API
---
