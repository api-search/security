---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: huckberry.com
  spf: true
hosts:
- cert_expires: Oct  7 15:34:26 2026 GMT
  host: huckberry.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Huckberry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huckberry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Huckberry
provider_slug: huckberry
slug: huckberry-domain-security
source_filename: huckberry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huckberry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:34:26 2026 GMT\n  hsts: null\ndomains:\n- domain: huckberry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huckberry/refs/heads/main/security/huckberry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Retail
- Direct to Consumer
- Apparel
- Outdoor
- Consumer Goods
- Media
---
