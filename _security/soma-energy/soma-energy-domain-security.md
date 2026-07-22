---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: soma.energy
  spf: true
hosts:
- cert_expires: Sep 24 21:55:20 2026 GMT
  host: soma.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soma Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soma Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Soma Energy
provider_slug: soma-energy
slug: soma-energy-domain-security
source_filename: soma-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soma.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:55:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: soma.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soma-energy/refs/heads/main/security/soma-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Energy
- Artificial Intelligence
- Energy Trading
- Battery Storage
- Data Centers
- Grid Optimization
- Clean Energy
---
