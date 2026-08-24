---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hero.co
  spf: true
hosts:
- cert_expires: Nov  7 03:33:47 2026 GMT
  host: www.hero.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 20:15:33 2026 GMT
  host: shop.hero.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hero Bread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hero Bread, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hero Bread
provider_slug: hero-bread
slug: hero-bread-domain-security
source_filename: hero-bread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hero.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 03:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shop.hero.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 20:15:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hero.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hero-bread/refs/heads/main/security/hero-bread-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agent Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Direct to Consumer
---
