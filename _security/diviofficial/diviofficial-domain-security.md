---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diviofficial.com
  spf: true
hosts:
- cert_expires: Sep  2 21:46:02 2026 GMT
  host: diviofficial.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diviofficial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Divi Official, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Divi Official
provider_slug: diviofficial
slug: diviofficial-domain-security
source_filename: diviofficial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diviofficial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:46:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: diviofficial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diviofficial/refs/heads/main/security/diviofficial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Beauty
- Haircare
- E-Commerce
- Direct to Consumer
- Shopify
- Subscription
---
