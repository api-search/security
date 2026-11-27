---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: movesurge.com
  spf: true
hosts:
- cert_expires: Jan 23 12:39:52 2027 GMT
  host: movesurge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MoveSurge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoveSurge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MoveSurge
provider_slug: movesurge-com
slug: movesurge-com-domain-security
source_filename: movesurge-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: movesurge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 12:39:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: movesurge.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/movesurge-com/security/movesurge-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Real-Time Data
- Stock Market
- News
- Alerts
---
