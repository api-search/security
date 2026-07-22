---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iamfy.co
  spf: true
hosts:
- cert_expires: Oct  1 04:26:35 2026 GMT
  host: iamfy.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fy
provider_slug: fy
slug: fy-domain-security
source_filename: fy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iamfy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:26:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: iamfy.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fy/refs/heads/main/security/fy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- E-Commerce
- Retail
- Wall Art
- Home Decor
- Consumer
- Shopify
---
