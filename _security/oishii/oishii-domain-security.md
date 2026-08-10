---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: oishii.com
  spf: false
hosts:
- cert_expires: Oct 30 09:21:32 2026 GMT
  host: oishii.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oishii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oishii, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Oishii
provider_slug: oishii
slug: oishii-domain-security
source_filename: oishii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oishii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 09:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: oishii.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oishii/refs/heads/main/security/oishii-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Agriculture
- Vertical Farming
- Food and Beverage
- Consumer Products
- Ecommerce
- Retail
- Agent Commerce
- Shopify
- MCP
- Universal Commerce Protocol
---
