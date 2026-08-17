---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vidjet.io
  spf: true
hosts:
- cert_expires: Nov 11 11:02:05 2026 GMT
  host: www.vidjet.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: help.vidjet.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: app-api.vidjet.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vidjet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vidjet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vidjet
provider_slug: vidjet
slug: vidjet-domain-security
source_filename: vidjet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vidjet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 11:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.vidjet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\n- host: app-api.vidjet.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vidjet.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidjet/refs/heads/main/security/vidjet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Video
- Shoppable Video
- Shopify
- Conversion
- Marketing
- No-code
- Widgets
- Embed
---
