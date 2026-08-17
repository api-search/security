---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flyingembers.com
  spf: true
hosts:
- cert_expires: Oct 28 21:37:01 2026 GMT
  host: www.flyingembers.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flying Embers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flying Embers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flying Embers
provider_slug: flying-embers
slug: flying-embers-domain-security
source_filename: flying-embers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flyingembers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 21:37:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: flyingembers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flying-embers/refs/heads/main/security/flying-embers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Beverages
- Consumer Packaged Goods
- Agentic Commerce
- MCP
- Shopify
- Direct to Consumer
---
