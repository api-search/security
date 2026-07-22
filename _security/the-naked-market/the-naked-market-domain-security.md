---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thenakedmarket.com
  spf: false
hosts:
- cert_expires: Sep 17 05:33:33 2026 GMT
  host: thenakedmarket.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Naked Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Naked Market, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: The Naked Market
provider_slug: the-naked-market
slug: the-naked-market-domain-security
source_filename: the-naked-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thenakedmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:33:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: thenakedmarket.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-naked-market/refs/heads/main/security/the-naked-market-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Consumer Packaged Goods
- Food and Beverage
- Direct to Consumer
- Snacks
- Brand Incubator
- E-Commerce
---
