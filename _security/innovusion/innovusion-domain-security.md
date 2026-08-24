---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seyond.com
  spf: true
hosts:
- cert_expires: Oct  4 21:33:08 2026 GMT
  host: seyond.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Innovusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seyond, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seyond
provider_slug: innovusion
slug: innovusion-domain-security
source_filename: innovusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seyond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:33:08 2026 GMT\n  hsts: false\ndomains:\n- domain: seyond.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovusion/refs/heads/main/security/innovusion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LiDAR
- Sensors
- Autonomous Driving
- Intelligent Transportation
- Robotics
- Perception
- Smart Cities
- Automotive
- Hardware
---
