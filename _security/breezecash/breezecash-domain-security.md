---
api_specs:
- filename: breezecash-customers-api-openapi.yml
  format: yaml
  label: Breeze.cash Customers API
  slug: breezecash-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-customers-api-openapi.yml
- filename: breezecash-direct-payment-api-openapi.yml
  format: yaml
  label: Breeze.cash Direct Payment API
  slug: breezecash-direct-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-direct-payment-api-openapi.yml
- filename: breezecash-disputes-api-openapi.yml
  format: yaml
  label: Breeze.cash Disputes API
  slug: breezecash-disputes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-disputes-api-openapi.yml
- filename: breezecash-fraud-reports-api-openapi.yml
  format: yaml
  label: Breeze.cash Fraud Reports API
  slug: breezecash-fraud-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-fraud-reports-api-openapi.yml
- filename: breezecash-headless-kyc-api-openapi.yml
  format: yaml
  label: Breeze.cash Headless KYC API
  slug: breezecash-headless-kyc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-headless-kyc-api-openapi.yml
- filename: breezecash-headless-payout-api-openapi.yml
  format: yaml
  label: Breeze.cash Headless Payout API
  slug: breezecash-headless-payout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-headless-payout-api-openapi.yml
- filename: breezecash-invoices-api-openapi.yml
  format: yaml
  label: Breeze.cash Invoices API
  slug: breezecash-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-invoices-api-openapi.yml
- filename: breezecash-liquidation-addresses-api-openapi.yml
  format: yaml
  label: Breeze.cash Liquidation Addresses API
  slug: breezecash-liquidation-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-liquidation-addresses-api-openapi.yml
- filename: breezecash-offramp-api-openapi.yml
  format: yaml
  label: Breeze.cash Offramp API
  slug: breezecash-offramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-offramp-api-openapi.yml
- filename: breezecash-payment-pages-api-openapi.yml
  format: yaml
  label: Breeze.cash Payment Pages API
  slug: breezecash-payment-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-payment-pages-api-openapi.yml
- filename: breezecash-payout-pages-api-openapi.yml
  format: yaml
  label: Breeze.cash Payout Pages API
  slug: breezecash-payout-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-payout-pages-api-openapi.yml
- filename: breezecash-products-api-openapi.yml
  format: yaml
  label: Breeze.cash Products API
  slug: breezecash-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-products-api-openapi.yml
- filename: breezecash-risk-api-openapi.yml
  format: yaml
  label: Breeze.cash Risk API
  slug: breezecash-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-risk-api-openapi.yml
- filename: breezecash-statements-api-openapi.yml
  format: yaml
  label: Breeze.cash Statements API
  slug: breezecash-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-statements-api-openapi.yml
- filename: breezecash-subscriptions-api-openapi.yml
  format: yaml
  label: Breeze.cash Subscriptions API
  slug: breezecash-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-subscriptions-api-openapi.yml
- filename: breezecash-tax-api-openapi.yml
  format: yaml
  label: Breeze.cash Tax API
  slug: breezecash-tax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-tax-api-openapi.yml
- filename: breezecash-webhooks-api-openapi.yml
  format: yaml
  label: Breeze.cash Webhooks API
  slug: breezecash-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: breeze.cash
  spf: true
hosts:
- cert_expires: Jan  8 07:50:04 2027 GMT
  host: breeze.cash
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breezecash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breeze.cash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Breeze.cash
provider_slug: breezecash
slug: breezecash-domain-security
source_filename: breezecash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breeze.cash\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 07:50:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: breeze.cash\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/breezecash/security/breezecash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- FinTech
- Payments
- Crypto
- Startup
- Venture-backed
---
