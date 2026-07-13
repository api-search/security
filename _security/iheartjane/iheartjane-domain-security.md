---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iheartjane.com
  spf: true
hosts:
- cert_expires: Oct  5 05:19:15 2026 GMT
  host: www.iheartjane.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 05:19:15 2026 GMT
  host: api.iheartjane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 05:19:15 2026 GMT
  host: dm-sdk-docs.iheartjane.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iheartjane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jane (iHeartJane), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jane (iHeartJane)
provider_slug: iheartjane
slug: iheartjane-domain-security
source_filename: iheartjane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iheartjane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:19:15 2026 GMT\n  hsts: false\n- host: api.iheartjane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:19:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dm-sdk-docs.iheartjane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:19:15 2026 GMT\n  hsts: false\ndomains:\n- domain: iheartjane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iheartjane/refs/heads/main/security/iheartjane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cannabis
- Ecommerce
- Marketplace
- Dispensary
- Menu
- Products
- Retail
- Point of Sale
- Personalization
---
