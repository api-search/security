---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: righthandrobotics.com
  spf: true
hosts:
- cert_expires: Sep 26 16:49:00 2026 GMT
  host: righthandrobotics.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Righthand Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RightHand Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RightHand Robotics
provider_slug: righthand-robotics
slug: righthand-robotics-domain-security
source_filename: righthand-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: righthandrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:49:00 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: righthandrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/righthand-robotics/refs/heads/main/security/righthand-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Robotics
- Warehouse Automation
- Order Fulfillment
- Piece Picking
- Logistics
- Machine Learning
---
