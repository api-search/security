---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: oatside.com
  spf: true
hosts:
- cert_expires: Oct 31 20:51:15 2026 GMT
  host: oatside.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 03:39:32 2026 GMT
  host: shop.oatside.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oatside Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oatside, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Oatside
provider_slug: oatside
slug: oatside-domain-security
source_filename: oatside-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oatside.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 20:51:15 2026 GMT\n  hsts: false\n- host: shop.oatside.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 03:39:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: oatside.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oatside/refs/heads/main/security/oatside-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Oat Milk
- Plant-Based
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Retail
- Singapore
- Southeast Asia
---
