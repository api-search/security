---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parser.club
  spf: true
hosts:
- cert_expires: Jan 13 06:46:18 2027 GMT
  host: parser.club
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parser Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parser Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Parser Club
provider_slug: parser-club
slug: parser-club-domain-security
source_filename: parser-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parser.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 06:46:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parser.club\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parser-club/security/parser-club-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Data Parsing
- Marketing Intelligence
- Telegram
- VK
- 2GIS
- Yandex Maps
- Wildberries
- Avito
---
