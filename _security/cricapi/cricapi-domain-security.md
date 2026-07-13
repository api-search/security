---
api_specs:
- filename: cricapi-cricket-data-api-openapi.yml
  format: yaml
  label: Cricket Data API
  slug: cricket-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cricapi/refs/heads/main/openapi/cricapi-cricket-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cricapi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cricketdata.org
  spf: true
hosts:
- cert_expires: Oct  3 06:16:06 2026 GMT
  host: www.cricapi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 10:45:39 2026 GMT
  host: cricketdata.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 14:45:47 2026 GMT
  host: api.cricapi.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cricapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CricAPI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CricAPI
provider_slug: cricapi
slug: cricapi-domain-security
source_filename: cricapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cricapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 06:16:06 2026 GMT\n  hsts: false\n- host: cricketdata.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 10:45:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.cricapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 14:45:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: cricapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cricketdata.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cricapi/refs/heads/main/security/cricapi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cricket
- Sports
- Live Scores
- Player Statistics
- Match Data
- Fantasy Cricket
- Ball-by-Ball
- Team Rankings
- Schedules
- Sports Data
---
