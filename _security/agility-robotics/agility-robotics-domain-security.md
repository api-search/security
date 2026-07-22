---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agilityrobotics.com
  spf: true
hosts:
- cert_expires: Sep 22 18:16:58 2026 GMT
  host: www.agilityrobotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agility Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agility Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agility Robotics
provider_slug: agility-robotics
slug: agility-robotics-domain-security
source_filename: agility-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agilityrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:16:58 2026 GMT\n  hsts: false\ndomains:\n- domain: agilityrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agility-robotics/refs/heads/main/security/agility-robotics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Robotics
- Humanoid Robots
- Bipedal Robots
- Industrial Automation
- Warehouse Automation
- Logistics
- Embodied AI
- Fleet Management
- Cloud Platform
- Digit
- Arc
- Manufacturing
- Hardware
---
