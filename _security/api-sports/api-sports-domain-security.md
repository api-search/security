---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: api-sports.io
  spf: true
hosts:
- cert_expires: Sep 29 13:56:51 2026 GMT
  host: api-sports.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API-Sports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: API-Sports
provider_slug: api-sports
slug: api-sports-domain-security
source_filename: api-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-sports.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:56:51 2026 GMT\n  hsts: null\ndomains:\n- domain: api-sports.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-sports/refs/heads/main/security/api-sports-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Baseball
- Basketball
- Cricket
- Football
- Ice Hockey
- MMA
- Real-Time
- Rugby
- Sports Data
- Statistics
- Tennis
---
