---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: vidjet.com
  spf: false
hosts:
- cert_expires: Oct 12 20:12:00 2026 GMT
  host: vidjet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vidjet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vidjet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Vidjet
provider_slug: vidjet
slug: vidjet-domain-security
source_filename: vidjet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vidjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 20:12:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vidjet.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidjet/refs/heads/main/security/vidjet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- E-commerce
- Video
- Shoppable Video
- Shopify
- Conversion
- Marketing
- No-code
---
