---
api_specs:
- filename: shopgo-authentication-api-openapi.yml
  format: yaml
  label: ShopGo Authentication API
  slug: shopgo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/openapi/shopgo-authentication-api-openapi.yml
- filename: shopgo-orders-api-openapi.yml
  format: yaml
  label: ShopGo Orders API
  slug: shopgo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/openapi/shopgo-orders-api-openapi.yml
- filename: shopgo-store-api-openapi.yml
  format: yaml
  label: ShopGo Store API
  slug: shopgo-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/openapi/shopgo-store-api-openapi.yml
- filename: shopgo-tenants-api-openapi.yml
  format: yaml
  label: ShopGo Tenants API
  slug: shopgo-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/openapi/shopgo-tenants-api-openapi.yml
- filename: shopgo-users-api-openapi.yml
  format: yaml
  label: ShopGo Users API
  slug: shopgo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/openapi/shopgo-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shopgo.me
  spf: true
hosts:
- cert_expires: Sep 30 22:57:13 2026 GMT
  host: shopgo.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShopGo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ShopGo
provider_slug: shopgo
slug: shopgo-domain-security
source_filename: shopgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopgo.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:57:13 2026 GMT\n  hsts: null\ndomains:\n- domain: shopgo.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopgo/refs/heads/main/security/shopgo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- E-Commerce
- Online Stores
- Payments
- Shipping
- Software-as-a-Service
- MENA
- Order
---
