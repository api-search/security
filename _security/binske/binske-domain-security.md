---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: binske.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: shopbinske.com
  spf: false
hosts:
- cert_expires: Sep 16 23:48:32 2026 GMT
  host: binske.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 06:49:02 2026 GMT
  host: shopbinske.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binske Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binske, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Binske
provider_slug: binske
slug: binske-domain-security
source_filename: binske-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: binske.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:48:32 2026 GMT\n  hsts: false\n- host: shopbinske.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 06:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: binske.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shopbinske.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binske/refs/heads/main/security/binske-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cannabis
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Retail
- Shopify
- Agent Commerce
- UCP
- MCP
- Storefront
---
