---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: poppyhandcraftedpopcorn.com
  spf: true
hosts:
- cert_expires: Oct 29 20:26:02 2026 GMT
  host: poppyhandcraftedpopcorn.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poppy Handcrafted Popcorn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poppy Handcrafted Popcorn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Poppy Handcrafted Popcorn
provider_slug: poppy-handcrafted-popcorn
slug: poppy-handcrafted-popcorn-domain-security
source_filename: poppy-handcrafted-popcorn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poppyhandcraftedpopcorn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 20:26:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: poppyhandcraftedpopcorn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poppy-handcrafted-popcorn/refs/heads/main/security/poppy-handcrafted-popcorn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Snacks
---
