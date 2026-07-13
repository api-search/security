---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aousd.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: openusd.org
  spf: false
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: aousd.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: openusd.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aousd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alliance for OpenUSD, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Alliance for OpenUSD
provider_slug: aousd
slug: aousd-domain-security
source_filename: aousd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aousd.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: openusd.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aousd.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: openusd.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aousd/refs/heads/main/security/aousd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- 3D
- Interoperability
- Linux Foundation
- Metaverse
- OpenUSD
- Specification
- Standards
- USD
- Visual Effects
---
