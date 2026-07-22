---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hillhousehome.com
  spf: true
hosts:
- cert_expires: Aug 25 22:39:33 2026 GMT
  host: hillhousehome.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hill House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hill House, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hill House
provider_slug: hill-house
slug: hill-house-domain-security
source_filename: hill-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hillhousehome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:39:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hillhousehome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hill-house/refs/heads/main/security/hill-house-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Retail
- Home Goods
- Apparel
- Direct to Consumer
- Consumer Brand
- Shopify
- MCP
---
