---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cerebelly.com
  spf: true
hosts:
- cert_expires: Sep 13 16:10:34 2026 GMT
  host: cerebelly.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerebelly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerebelly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cerebelly
provider_slug: cerebelly
slug: cerebelly-domain-security
source_filename: cerebelly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cerebelly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:10:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: cerebelly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebelly/refs/heads/main/security/cerebelly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Baby Food
- Consumer Packaged Goods
- Food and Beverage
- eCommerce
- Retail
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Nutrition
---
