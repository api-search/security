---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cricket-api.net
  spf: false
hosts:
- cert_expires: Oct 28 16:40:11 2026 GMT
  host: cricket-api.net
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cricket Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cricket API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Cricket API
provider_slug: cricket-api
slug: cricket-api-domain-security
source_filename: cricket-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cricket-api.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 16:40:11 2026 GMT\n  hsts: false\ndomains:\n- domain: cricket-api.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cricket-api/refs/heads/main/security/cricket-api-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Cricket
- Sports
- Sports Data
- Live Scores
- Cricket Statistics
- Cricket Odds
- Cricket Predictions
---
