---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: api-football.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: api-sports.io
  spf: true
hosts:
- cert_expires: Nov 12 19:25:09 2026 GMT
  host: www.api-football.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 06:49:24 2026 GMT
  host: v3.football.api-sports.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Football Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Football, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: API Football
provider_slug: api-football
slug: api-football-domain-security
source_filename: api-football-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.api-football.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 19:25:09 2026 GMT\n  hsts: null\n- host: v3.football.api-sports.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 06:49:24 2026 GMT\n  hsts: null\ndomains:\n- domain: api-football.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: api-sports.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-football/refs/heads/main/security/api-football-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports
- Football
- Soccer
- Live Scores
- Statistics
---
