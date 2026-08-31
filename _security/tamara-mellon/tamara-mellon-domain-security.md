---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tamaramellon.com
  spf: true
hosts:
- cert_expires: Oct 14 09:32:31 2026 GMT
  host: shop.tamaramellon.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tamara Mellon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tamara Mellon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tamara Mellon
provider_slug: tamara-mellon
slug: tamara-mellon-domain-security
source_filename: tamara-mellon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shop.tamaramellon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: tamaramellon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamara-mellon/refs/heads/main/security/tamara-mellon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- Footwear
- Luxury
- Retail
- Direct to Consumer
- E-Commerce
- Consumer Goods
- Apparel
---
