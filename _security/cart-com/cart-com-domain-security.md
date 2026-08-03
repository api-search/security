---
api_specs:
- filename: cart-com-online-store-openapi-original.yml
  format: yaml
  label: Cart.com Online Store API
  slug: online-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cart-com/refs/heads/main/openapi/cart-com-online-store-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cart.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: americommerce.com
  spf: true
hosts:
- cert_expires: Oct 10 14:01:02 2026 GMT
  host: cart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 09:42:11 2026 GMT
  host: developers.cart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:29:03 2026 GMT
  host: www.americommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cart Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cart.com, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cart.com
provider_slug: cart-com
slug: cart-com-domain-security
source_filename: cart-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 09:42:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.americommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:29:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: americommerce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cart-com/refs/heads/main/security/cart-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Commerce
- Retail
- Order Management
- Fulfillment
- Logistics
- Marketplaces
- Storefront
- Catalog
- Shipping
---
