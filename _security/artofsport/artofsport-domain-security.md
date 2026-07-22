---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: artofsport.com
  spf: true
hosts:
- cert_expires: Aug 28 06:31:35 2026 GMT
  host: artofsport.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artofsport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artofsport, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Artofsport
provider_slug: artofsport
slug: artofsport-domain-security
source_filename: artofsport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artofsport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 06:31:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: artofsport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artofsport/refs/heads/main/security/artofsport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Personal Care
- Skincare
- Body Care
- Athletics
- Direct to Consumer
- E-commerce
- Shopify
---
