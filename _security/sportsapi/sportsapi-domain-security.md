---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sportsapi.com
  spf: true
hosts:
- cert_expires: Aug 23 18:33:13 2026 GMT
  host: sportsapi.com
  hsts: true
  hsts_max_age: 5
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportsapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SportsAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SportsAPI
provider_slug: sportsapi
slug: sportsapi-domain-security
source_filename: sportsapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:33:13 2026 GMT\n  hsts: true\n  hsts_max_age: 5\ndomains:\n- domain: sportsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsapi/refs/heads/main/security/sportsapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports
- Sports Data
- API Directory
- Comparison
---
