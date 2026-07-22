---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tennibot.com
  spf: true
hosts:
- cert_expires: Sep  5 03:03:49 2026 GMT
  host: tennibot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tennibot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tennibot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tennibot
provider_slug: tennibot
slug: tennibot-domain-security
source_filename: tennibot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tennibot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tennibot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tennibot/refs/heads/main/security/tennibot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Computer Vision
- Sports Technology
- Tennis
- Pickleball
- Padel
- Consumer Hardware
- Mobile App
---
