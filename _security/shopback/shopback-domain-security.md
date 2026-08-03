---
api_specs:
- filename: shopback-online-payments-openapi.yml
  format: yaml
  label: ShopBack Online Payments API
  slug: shopback-online-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/openapi/shopback-online-payments-openapi.yml
- filename: shopback-in-store-payments-openapi.yml
  format: yaml
  label: ShopBack In-Store Payments API
  slug: shopback-in-store-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/openapi/shopback-in-store-payments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopback.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hoolah.co
  spf: true
hosts:
- cert_expires: Oct  4 06:58:02 2026 GMT
  host: www.shopback.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 20:52:34 2026 GMT
  host: docs.shopback.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 07:54:49 2026 GMT
  host: prod-merchant-service.hoolah.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopback Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShopBack, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ShopBack
provider_slug: shopback
slug: shopback-domain-security
source_filename: shopback-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shopback.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:58:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.shopback.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:52:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod-merchant-service.hoolah.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 07:54:49 2026 GMT\n  hsts: null\ndomains:\n- domain: shopback.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hoolah.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopback/refs/heads/main/security/shopback-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Cashback
- Rewards
- Loyalty
- E-Commerce
- Buy Now Pay Later
- Point Of Sale
- Checkout
- Singapore
---
