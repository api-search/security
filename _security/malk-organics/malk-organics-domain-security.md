---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: malkorganics.com
  spf: true
hosts:
- cert_expires: Sep 30 19:07:02 2026 GMT
  host: malkorganics.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Malk Organics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MALK Organics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MALK Organics
provider_slug: malk-organics
slug: malk-organics-domain-security
source_filename: malk-organics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: malkorganics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:07:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: malkorganics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/malk-organics/refs/heads/main/security/malk-organics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Food and Beverage
- Consumer Packaged Goods
- Plant-Based
- Organic
- Direct to Consumer
- Agent Commerce
- MCP
- Shopify
---
