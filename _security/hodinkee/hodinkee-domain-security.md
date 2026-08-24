---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hodinkee.com
  spf: true
hosts:
- cert_expires: Nov  4 12:26:42 2026 GMT
  host: www.hodinkee.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 12:15:32 2026 GMT
  host: shop.hodinkee.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hodinkee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hodinkee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hodinkee
provider_slug: hodinkee
slug: hodinkee-domain-security
source_filename: hodinkee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hodinkee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 12:26:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: shop.hodinkee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:15:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hodinkee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hodinkee/refs/heads/main/security/hodinkee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Watches
- Luxury Goods
- E-Commerce
- Media
- Publishing
- Retail
- Agentic Commerce
- Model Context Protocol
- Shopify
---
