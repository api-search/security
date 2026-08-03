---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: misorobotics.com
  spf: true
hosts:
- cert_expires: Oct 11 03:35:24 2026 GMT
  host: www.misorobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Miso Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miso Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Miso Robotics
provider_slug: miso-robotics
slug: miso-robotics-domain-security
source_filename: miso-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.misorobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 03:35:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: misorobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miso-robotics/refs/heads/main/security/miso-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Kitchen Automation
- Restaurants
- Food Service
- Artificial Intelligence
- Computer Vision
- Workforce Management
- Point of Sale
---
