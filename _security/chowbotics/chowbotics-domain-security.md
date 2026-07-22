---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chowbotics.com
  spf: false
hosts:
- cert_expires: Sep 15 00:17:34 2026 GMT
  host: chowbotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chowbotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chowbotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: chowbotics
provider_slug: chowbotics
slug: chowbotics-domain-security
source_filename: chowbotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chowbotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:17:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chowbotics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chowbotics/refs/heads/main/security/chowbotics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Food Technology
- Foodservice
- Automation
- Acquired
- DoorDash
---
