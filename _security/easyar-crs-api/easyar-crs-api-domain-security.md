---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: easyar.com
  spf: false
hosts:
- cert_expires: Dec  7 02:47:03 2026 GMT
  host: help.easyar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 02:47:03 2026 GMT
  host: uac.easyar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Easyar Crs Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasyAR CRS API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: EasyAR CRS API
provider_slug: easyar-crs-api
slug: easyar-crs-api-domain-security
source_filename: easyar-crs-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.easyar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:47:03 2026 GMT\n  hsts: false\n- host: uac.easyar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:47:03 2026 GMT\n  hsts: null\ndomains:\n- domain: easyar.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyar-crs-api/refs/heads/main/security/easyar-crs-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Augmented Reality
- ar-sdk
- Cloud Recognition
- Image Recognition
- Spatial Computing
- Visual Positioning
- Computer-Vision
- Developer Tools
---
