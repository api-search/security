---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arcturus.io
  spf: false
hosts:
- cert_expires: Aug 28 23:21:37 2026 GMT
  host: arcturus.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arcturus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcturus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Arcturus
provider_slug: arcturus
slug: arcturus-domain-security
source_filename: arcturus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcturus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:21:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arcturus.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcturus/refs/heads/main/security/arcturus-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Advanced Materials
- Carbon Nanomaterials
- Energy
- Climate Tech
- Hardware
- Deep Tech
---
