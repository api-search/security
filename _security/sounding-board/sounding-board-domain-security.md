---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soundingboardinc.com
  spf: true
hosts:
- cert_expires: Sep  1 23:47:35 2026 GMT
  host: www.soundingboardinc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sounding Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sounding Board, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sounding Board
provider_slug: sounding-board
slug: sounding-board-domain-security
source_filename: sounding-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soundingboardinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:47:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: soundingboardinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sounding-board/refs/heads/main/security/sounding-board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Leadership Development
- Coaching
- Mentoring
- Talent Development
- Human Resources
- SaaS
---
