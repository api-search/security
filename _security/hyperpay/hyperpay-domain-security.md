---
api_specs:
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay COPYandPAY API
  slug: hyperpay-copyandpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Server-to-Server Payments API
  slug: hyperpay-server-to-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Registration Tokens API
  slug: hyperpay-registration-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Query API
  slug: hyperpay-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
description: ''
domains: []
hosts:
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: www.hyperpay.com
  hsts: false
  http_status: 200
  https: true
- host: hyperpay.com
  http_status: 301
  https: true
  note: Redirects to www.hyperpay.com.
- cert_expires: Aug 11 00:52:34 2026 GMT
  host: eu-prod.oppwa.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 200
  https: true
  note: Production (live) API host of the ACI / OPPWA platform HyperPay runs on.
- cert_expires: Aug 11 00:52:34 2026 GMT
  host: test.oppwa.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 200
  https: true
  note: Integration / test API host.
- host: hyperpay.docs.oppwa.com
  http_status: 200
  https: true
  note: Developer documentation portal.
kind: domain-security
layout: security
method: probed
name: Hyperpay Domain Security
name_suffix: Domain Security
overview: Domain security posture for HyperPay, probed live across 5 host(s) and 0 registrable domain(s). 5 host(s) serve HTTPS; 2 advertise HSTS.
provider_name: HyperPay
provider_slug: hyperpay
slug: hyperpay-domain-security
source_filename: hyperpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperpay.com\n  https: true\n  http_status: 200\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: false\n- host: hyperpay.com\n  https: true\n  http_status: 301\n  note: Redirects to www.hyperpay.com.\n- host: eu-prod.oppwa.com\n  https: true\n  http_status: 200\n  cert_expires: Aug 11 00:52:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Production (live) API host of the ACI / OPPWA platform HyperPay runs on.\n- host: test.oppwa.com\n  https: true\n  http_status: 200\n  cert_expires: Aug 11 00:52:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Integration / test API host.\n- host: hyperpay.docs.oppwa.com\n  https: true\n  http_status: 200\n  note: Developer documentation portal.\nnotes: >-\n  API traffic terminates on\
  \ the ACI / OPPWA hosts (eu-prod.oppwa.com live,\n  test.oppwa.com test), which enforce HSTS with a two-year max-age, subdomain\n  inclusion, and preload. All payment operations require TLS. HyperPay is a\n  PCI-DSS Level 1 certified payment service provider; using the COPYandPAY widget\n  keeps raw card data off the merchant server, while Server-to-Server requires the\n  merchant to hold PCI-DSS scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/security/hyperpay-domain-security.yml
summary_line: HSTS
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- Saudi Arabia
- mada
- Apple Pay
- Cards
---
