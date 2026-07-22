---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transform.co
  spf: false
hosts:
- cert_expires: Sep 21 12:18:15 2026 GMT
  host: transform.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Transform
provider_slug: transform
slug: transform-domain-security
source_filename: transform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transform.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:18:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: transform.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transform/refs/heads/main/security/transform-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Metrics
- Semantic Layer
- Analytics
- Data
- Business Intelligence
- Acquired
---
