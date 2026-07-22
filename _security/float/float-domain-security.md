---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: float.build
  spf: true
hosts:
- cert_expires: Sep 18 04:03:46 2026 GMT
  host: float.build
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Float Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for float, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: float
provider_slug: float
slug: float-domain-security
source_filename: float-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: float.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: float.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/float/refs/heads/main/security/float-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Product Studio
- Design
- Software
- Video
- Startup
- Consumer
---
