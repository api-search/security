---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mudwtr.com
  spf: true
hosts:
- cert_expires: Oct 26 20:10:02 2026 GMT
  host: mudwtr.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mud Wtr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mud\Wtr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mud\Wtr
provider_slug: mud-wtr
slug: mud-wtr-domain-security
source_filename: mud-wtr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mudwtr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 20:10:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: mudwtr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mud-wtr/refs/heads/main/security/mud-wtr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Consumer Goods
- Food and Beverage
- Shopify
- Agentic Commerce
- MCP
- GraphQL
- UCP
---
