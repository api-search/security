---
api_specs:
- filename: the-odds-api-openapi.yml
  format: yaml
  label: The Odds API
  slug: the-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/openapi/the-odds-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: the-odds-api.com
  spf: true
hosts:
- cert_expires: Sep 20 22:18:20 2026 GMT
  host: the-odds-api.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.the-odds-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: ipv6-api.the-odds-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Odds Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Odds API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Odds API
provider_slug: the-odds-api
slug: the-odds-api-domain-security
source_filename: the-odds-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-odds-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:18:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.the-odds-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n- host: ipv6-api.the-odds-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: the-odds-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/security/the-odds-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Betting
- Odds
- Sports
- Scores
- Historical Data
---
