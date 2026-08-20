---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bartesian.com
  spf: true
hosts:
- cert_expires: Oct 27 15:41:33 2026 GMT
  host: bartesian.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bartesian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bartesian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bartesian
provider_slug: bartesian
slug: bartesian-domain-security
source_filename: bartesian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bartesian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 15:41:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: bartesian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bartesian/refs/heads/main/security/bartesian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Consumer Products
- Appliances
- Beverages
- Direct to Consumer
- Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
