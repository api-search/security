---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kitro.ch
  spf: true
hosts:
- cert_expires: Sep  4 14:12:15 2026 GMT
  host: kitro.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kitro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KITRO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: KITRO
provider_slug: kitro
slug: kitro-domain-security
source_filename: kitro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitro.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:12:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kitro.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitro/refs/heads/main/security/kitro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Food Waste
- Sustainability
- Hospitality
- Food Service
- Analytics
- Artificial Intelligence
- Computer Vision
- Internet of Things
- Switzerland
---
