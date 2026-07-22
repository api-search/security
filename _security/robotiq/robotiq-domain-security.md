---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: robotiq.com
  spf: true
hosts:
- cert_expires: Sep 15 06:41:19 2026 GMT
  host: robotiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robotiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robotiq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Robotiq
provider_slug: robotiq
slug: robotiq-domain-security
source_filename: robotiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robotiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:41:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: robotiq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robotiq/refs/heads/main/security/robotiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Automation
- Manufacturing
- Collaborative Robots
- Grippers
- End-of-Arm Tooling
- Palletizing
- Machine Tending
- Sensors
- Hardware
---
