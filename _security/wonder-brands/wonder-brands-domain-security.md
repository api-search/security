---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wonderbrands.co
  spf: true
hosts:
- cert_expires: Aug 29 05:10:15 2026 GMT
  host: wonderbrands.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wonder Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wonder Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wonder Brands
provider_slug: wonder-brands
slug: wonder-brands-domain-security
source_filename: wonder-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wonderbrands.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:10:15 2026 GMT\n  hsts: false\ndomains:\n- domain: wonderbrands.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonder-brands/refs/heads/main/security/wonder-brands-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ecommerce
- E-Commerce
- Consumer Goods
- Retail
- Brand Aggregator
- Latin America
- Direct To Consumer
---
