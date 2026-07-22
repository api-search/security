---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbanmachine.build
  spf: false
hosts:
- cert_expires: Oct 19 12:17:05 2026 GMT
  host: urbanmachine.build
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urban Machine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Machine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Urban Machine
provider_slug: urban-machine
slug: urban-machine-domain-security
source_filename: urban-machine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanmachine.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 12:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: urbanmachine.build\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-machine/refs/heads/main/security/urban-machine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Robotics
- Construction
- Wood Reclamation
- Circular Economy
- Computer Vision
---
