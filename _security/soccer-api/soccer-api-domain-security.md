---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soccer-api.com
  spf: false
hosts:
- cert_expires: Nov  4 04:57:40 2026 GMT
  host: soccer-api.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Soccer Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soccer API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Soccer API
provider_slug: soccer-api
slug: soccer-api-domain-security
source_filename: soccer-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soccer-api.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 04:57:40 2026 GMT\n  hsts: false\ndomains:\n- domain: soccer-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soccer-api/refs/heads/main/security/soccer-api-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Sports
- Football
- Live Scores
- Odds
- Predictions
- Sports Data
- Statistics
---
