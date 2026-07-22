---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cleanliquor.com
  spf: true
hosts:
- cert_expires: Aug 29 00:11:31 2026 GMT
  host: www.cleanliquor.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cleanco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CleanCo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CleanCo
provider_slug: cleanco
slug: cleanco-domain-security
source_filename: cleanco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cleanliquor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:11:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: cleanliquor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanco/refs/heads/main/security/cleanco-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Beverage
- Spirits
- Non-Alcoholic
- Low-Alcohol
- Consumer Packaged Goods
- Direct to Consumer
- Retail
---
