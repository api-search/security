---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liveouter.com
  spf: true
hosts:
- cert_expires: Oct 26 06:10:33 2026 GMT
  host: liveouter.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Outer
provider_slug: outer
slug: outer-domain-security
source_filename: outer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liveouter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 06:10:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: liveouter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outer/refs/heads/main/security/outer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Consumer Goods
- Furniture
- Homes
- Direct to Consumer
- Agentic Commerce
- Shopify
- Universal Commerce Protocol
---
