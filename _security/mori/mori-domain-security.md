---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: babymori.com
  spf: true
hosts:
- cert_expires: Aug 27 08:33:34 2026 GMT
  host: babymori.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MORI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MORI
provider_slug: mori
slug: mori-domain-security
source_filename: mori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: babymori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 08:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: babymori.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mori/refs/heads/main/security/mori-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-commerce
- Baby Products
- Consumer Goods
- Apparel
- Direct to Consumer
- Shopify
- MCP
- Agent Native
- Universal Commerce Protocol
---
