---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shippingbo.com
  spf: true
hosts:
- cert_expires: Sep 23 05:50:23 2026 GMT
  host: www.shippingbo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:21:59 2026 GMT
  host: developer.shippingbo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shippingbo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shippingbo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shippingbo
provider_slug: shippingbo
slug: shippingbo-domain-security
source_filename: shippingbo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shippingbo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:50:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.shippingbo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:21:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shippingbo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippingbo/refs/heads/main/security/shippingbo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Logistics
- Ecommerce
- Order Management
- Warehouse Management
- Transport Management
- OMS
- WMS
- TMS
- Multi-Carrier
- Fulfillment
- 3PL
- Marketplaces
- Webhooks
- OAuth2
- SaaS
- France
- French Tech
---
