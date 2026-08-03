---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mammothbrands.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: harrys.com
  spf: true
hosts:
- cert_expires: Sep  6 21:03:23 2026 GMT
  host: www.mammothbrands.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:19:32 2026 GMT
  host: www.harrys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 07:17:02 2026 GMT
  host: www.shopflamingo.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harry S Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mammoth Brands, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mammoth Brands
provider_slug: harry-s
slug: harry-s-domain-security
source_filename: harry-s-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mammothbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:03:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.harrys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.shopflamingo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:17:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: mammothbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: harrys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harry-s/refs/heads/main/security/harry-s-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Retail
- E-Commerce
- Personal Care
- Agentic Commerce
- Model Context Protocol
- Shopify
---
