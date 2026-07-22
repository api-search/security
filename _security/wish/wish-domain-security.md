---
api_specs:
- filename: wish-marketplace-v3-openapi.json
  format: json
  label: Wish Marketplace V3 API
  slug: wish-marketplace-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-marketplace-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wish.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: wish.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 11:28:29 2026 GMT
  host: china-merchant.wish.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 11:28:29 2026 GMT
  host: merchant.wish.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wish, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wish
provider_slug: wish
slug: wish-domain-security
source_filename: wish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\n- host: china-merchant.wish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 11:28:29 2026 GMT\n  hsts: null\n- host: merchant.wish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 11:28:29 2026 GMT\n  hsts: null\ndomains:\n- domain: wish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/security/wish-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Merchants
- Orders
- Products
- Fulfillment
- Shopping
- OAuth
---
