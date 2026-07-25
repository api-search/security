---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: youi.com.au
  spf: true
hosts:
- cert_expires: Sep 13 20:06:44 2026 GMT
  host: www.youi.com.au
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Youi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Youi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Youi
provider_slug: youi
slug: youi-domain-security
source_filename: youi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.youi.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:06:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: youi.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youi/refs/heads/main/security/youi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Property and Casualty
- General Insurance
- Motor Insurance
- Home Insurance
- Business Insurance
- Compulsory Third Party
- Carrier
- Direct to Consumer
- No Public API
---
