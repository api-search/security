---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aes.com
  spf: true
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fluenceenergy.com
  spf: true
hosts:
- cert_expires: Sep 16 01:48:05 2026 GMT
  host: www.aes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 19:19:30 2026 GMT
  host: fluenceenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AES Corporation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AES Corporation
provider_slug: aes
slug: aes-domain-security
source_filename: aes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: fluenceenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:19:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fluenceenergy.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aes/refs/heads/main/security/aes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Power Generation
- Renewable Energy
- Battery Storage
- Utility
- Clean Energy
- Fortune 500
---
