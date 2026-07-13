---
api_specs:
- filename: wager-api-openapi.yml
  format: yaml
  label: Wager API - Sports Odds
  slug: wager-api-odds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/openapi/wager-api-openapi.yml
- filename: wager-api-openapi.yml
  format: yaml
  label: Wager API - Fantasy Sports Data
  slug: wager-api-fantasy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/openapi/wager-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wagerapi.com
  spf: false
hosts:
- cert_expires: Aug 13 19:24:09 2026 GMT
  host: wagerapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.wagerapi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wager Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wager API, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Wager API
provider_slug: wager-api
slug: wager-api-domain-security
source_filename: wager-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wagerapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 19:24:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wagerapi.com\n  https: false\ndomains:\n- domain: wagerapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/security/wager-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports Betting
- Sports Odds
- Fantasy Sports
- Sports Data
- NFL
- NBA
- MLB
- NHL
- NCAA
---
