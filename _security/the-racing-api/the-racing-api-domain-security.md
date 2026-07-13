---
api_specs:
- filename: the-racing-api-openapi.yml
  format: yaml
  label: The Racing API
  slug: the-racing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-racing-api/refs/heads/main/openapi/the-racing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theracingapi.com
  spf: true
hosts:
- cert_expires: Aug 20 20:01:30 2026 GMT
  host: www.theracingapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 20:01:30 2026 GMT
  host: api.theracingapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Racing Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Racing API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Racing API
provider_slug: the-racing-api
slug: the-racing-api-domain-security
source_filename: the-racing-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theracingapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 20:01:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.theracingapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 20:01:30 2026 GMT\n  hsts: null\ndomains:\n- domain: theracingapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-racing-api/refs/heads/main/security/the-racing-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Horse Racing
- Sports
- Statistics
- Betting
- Analytics
---
