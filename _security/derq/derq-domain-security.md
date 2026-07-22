---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: derq.com
  spf: true
hosts:
- cert_expires: Sep 26 03:04:12 2026 GMT
  host: derq.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Derq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Derq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Derq
provider_slug: derq
slug: derq-domain-security
source_filename: derq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: derq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:04:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: derq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/derq/refs/heads/main/security/derq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Intelligent Transportation
- Road Safety
- Traffic Analytics
- Computer Vision
- V2X
- Smart Cities
- Machine Learning
---
