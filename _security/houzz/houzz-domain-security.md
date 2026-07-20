---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: houzz.com
  spf: true
hosts:
- cert_expires: Jan 15 04:37:52 2027 GMT
  host: houzz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Houzz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Houzz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Houzz
provider_slug: houzz
slug: houzz-domain-security
source_filename: houzz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: houzz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 04:37:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: houzz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houzz/refs/heads/main/security/houzz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Marketplace
- Home Improvement
- Interior Design
- Home Renovation
- Furniture
- SaaS
---
