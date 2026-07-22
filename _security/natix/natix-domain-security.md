---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: natix.network
  spf: true
hosts:
- cert_expires: Oct 15 04:16:54 2026 GMT
  host: natix.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Natix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NATIX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NATIX
provider_slug: natix
slug: natix-domain-security
source_filename: natix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: natix.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: natix.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natix/refs/heads/main/security/natix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DePIN
- Mapping
- Autonomous Driving
- Physical AI
- Geospatial
- Computer Vision
- Web3
- Data
---
