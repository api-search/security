---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carbonrobotics.com
  spf: true
hosts:
- cert_expires: Oct  8 09:59:41 2026 GMT
  host: carbonrobotics.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbonrobotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carbon Robotics
provider_slug: carbonrobotics
slug: carbonrobotics-domain-security
source_filename: carbonrobotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbonrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:59:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: carbonrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbonrobotics/refs/heads/main/security/carbonrobotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Agriculture
- AgTech
- Artificial Intelligence
- Computer Vision
- Automation
- Autonomous Vehicles
---
