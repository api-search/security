---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 6thsense.dev
  spf: true
hosts:
- cert_expires: Sep 30 21:31:25 2026 GMT
  host: 6thsense.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 6Thsense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6thSense, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 6thSense
provider_slug: 6thsense
slug: 6thsense-domain-security
source_filename: 6thsense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 6thsense.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:31:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 6thsense.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6thsense/refs/heads/main/security/6thsense-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Physical AI
- Tactile Sensing
- Hardware
- Machine Learning
- Datasets
- Robot Manipulation
- Sensors
- Y Combinator
---
