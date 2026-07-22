---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: octavesecurity.com
  spf: false
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: octavesecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 13:48:02 2026 GMT
  host: portal.octavesecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qognify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qognify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Qognify
provider_slug: qognify
slug: qognify-domain-security
source_filename: qognify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octavesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.octavesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: octavesecurity.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qognify/refs/heads/main/security/qognify-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Physical Security
- Video Management System
- Video Surveillance
- PSIM
- Video Analytics
- Critical Infrastructure
- Enterprise Security
---
