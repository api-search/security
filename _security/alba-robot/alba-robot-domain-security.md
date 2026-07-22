---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alba-robot.com
  spf: true
hosts:
- cert_expires: Sep 23 09:06:31 2026 GMT
  host: alba-robot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alba Robot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alba Robot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alba Robot
provider_slug: alba-robot
slug: alba-robot-domain-security
source_filename: alba-robot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alba-robot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:06:31 2026 GMT\n  hsts: false\ndomains:\n- domain: alba-robot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alba-robot/refs/heads/main/security/alba-robot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Autonomous Mobility
- Micro-Mobility
- Airports
- Fleet Management
- Digital Twin
- Italy
---
