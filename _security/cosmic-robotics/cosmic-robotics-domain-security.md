---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosmicrobotics.com
  spf: true
hosts:
- cert_expires: Sep  6 08:32:22 2026 GMT
  host: www.cosmicrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cosmic Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmic Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cosmic Robotics
provider_slug: cosmic-robotics
slug: cosmic-robotics-domain-security
source_filename: cosmic-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cosmicrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cosmicrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmic-robotics/refs/heads/main/security/cosmic-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Construction Technology
- Automation
- Solar Energy
- Autonomous Systems
- Fleet Management
- Y Combinator
---
