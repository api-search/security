---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: any-api.com
  spf: false
hosts:
- cert_expires: Oct  5 02:08:54 2026 GMT
  host: any-api.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nba Stats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NBA Stats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NBA Stats
provider_slug: nba-stats
slug: nba-stats-domain-security
source_filename: nba-stats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: any-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: any-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nba-stats/refs/heads/main/security/nba-stats-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports And Fitness
- Public APIs
---
