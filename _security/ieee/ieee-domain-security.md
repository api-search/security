---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ieee.org
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: ieeexplore.ieee.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 20:56:04 2027 GMT
  host: developer.ieee.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 20:56:04 2027 GMT
  host: ieeexploreapi.ieee.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ieee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IEEE Xplore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IEEE Xplore
provider_slug: ieee
slug: ieee-domain-security
source_filename: ieee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ieeexplore.ieee.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ieee.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 20:56:04 2027 GMT\n  hsts: false\n- host: ieeexploreapi.ieee.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 20:56:04 2027 GMT\n  hsts: null\ndomains:\n- domain: ieee.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ieee/refs/heads/main/security/ieee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Science And Math
- Scholarly Publishing
- Engineering
- Computer Science
- Standards
- Research
- Academic
- Technology
---
