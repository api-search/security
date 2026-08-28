---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pragmaticsemi.com
  spf: true
hosts:
- cert_expires: Oct 16 07:24:14 2026 GMT
  host: www.pragmaticsemi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: portal.pragmaticsemi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api-portal.pragmaticsemi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pragmatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pragmatic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pragmatic
provider_slug: pragmatic
slug: pragmatic-domain-security
source_filename: pragmatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pragmaticsemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 07:24:14 2026 GMT\n  hsts: false\n- host: portal.pragmaticsemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-portal.pragmaticsemi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pragmaticsemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pragmatic/refs/heads/main/security/pragmatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Hardware
- Manufacturing
- Flexible Electronics
- Integrated Circuits
- Foundry
- NFC
- RFID
- Internet of Things
- United Kingdom
---
