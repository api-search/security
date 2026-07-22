---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: andromedarobotics.ai
  spf: false
hosts:
- cert_expires: Aug 29 06:00:57 2026 GMT
  host: andromedarobotics.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Andromeda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andromeda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Andromeda
provider_slug: andromeda
slug: andromeda-domain-security
source_filename: andromeda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andromedarobotics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:00:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: andromedarobotics.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andromeda/refs/heads/main/security/andromeda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Humanoid Robots
- Aged Care
- Assisted Living
- Elder Care
- AI Companion
- Healthcare
---
