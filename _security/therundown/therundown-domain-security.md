---
api_specs:
- filename: list-all-sports
  format: yaml
  label: TheRundown Sports Odds API
  slug: sports-odds-api
  spec_type: OpenAPI
  url: https://docs.therundown.io/api-reference/generated/v2-sports/list-all-sports
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: therundown.io
  spf: true
hosts:
- cert_expires: Sep  8 04:28:38 2026 GMT
  host: therundown.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Therundown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Rundown, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Rundown
provider_slug: therundown
slug: therundown-domain-security
source_filename: therundown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: therundown.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:28:38 2026 GMT\n  hsts: false\ndomains:\n- domain: therundown.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/security/therundown-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports
- Betting
- Odds
- NFL
- NBA
- MLB
- NHL
- Soccer
- Real-Time
- Sports Data
- Sportsbook
---
