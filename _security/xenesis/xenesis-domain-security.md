---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xenesis.io
  spf: true
hosts:
- cert_expires: Nov  9 11:02:54 2026 GMT
  host: xenesis.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xenesis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xenesis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Xenesis
provider_slug: xenesis
slug: xenesis-domain-security
source_filename: xenesis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xenesis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 11:02:54 2026 GMT\n  hsts: null\ndomains:\n- domain: xenesis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xenesis/refs/heads/main/security/xenesis-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Space
- Satellite
- Optical Communications
- Free Space Optics
- Laser Communications
- Telecommunications
- Aerospace
- Defense
- Connectivity
---
