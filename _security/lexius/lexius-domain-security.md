---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lexius.ai
  spf: true
hosts:
- cert_expires: Sep 24 07:07:57 2026 GMT
  host: www.lexius.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lexius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lexius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lexius
provider_slug: lexius
slug: lexius-domain-security
source_filename: lexius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lexius.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 07:07:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lexius.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexius/refs/heads/main/security/lexius-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Loss Prevention
- Retail
- Physical Security
- Computer Vision
- Video Analytics
- Theft Detection
- Artificial Intelligence
- Retail Technology
---
