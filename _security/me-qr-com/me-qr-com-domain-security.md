---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: me-qr.com
  spf: true
hosts:
- cert_expires: Feb  9 11:28:04 2027 GMT
  host: me-qr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ME-QR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ME-QR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ME-QR
provider_slug: me-qr-com
slug: me-qr-com-domain-security
source_filename: me-qr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: me-qr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 11:28:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: me-qr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/me-qr-com/security/me-qr-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- QR Code Generator
- Dynamic QR
- QR Templates
- QR Analytics
- Bulk QR Creation
- API Integration
---
