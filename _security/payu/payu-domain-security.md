---
api_specs:
- filename: payu-authorize-api-openapi.yml
  format: yaml
  label: PayU Authorize API
  slug: payu-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-authorize-api-openapi.yml
- filename: payu-card-installments-api-openapi.yml
  format: yaml
  label: PayU Card Installments API
  slug: payu-card-installments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-card-installments-api-openapi.yml
- filename: payu-fx-reference-api-openapi.yml
  format: yaml
  label: PayU FX-Reference API
  slug: payu-fx-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-fx-reference-api-openapi.yml
- filename: payu-marketplace-seller-api-openapi.yml
  format: yaml
  label: PayU Marketplace-Seller API
  slug: payu-marketplace-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-marketplace-seller-api-openapi.yml
- filename: payu-marketplace-verification-api-openapi.yml
  format: yaml
  label: PayU Marketplace-Verification API
  slug: payu-marketplace-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-marketplace-verification-api-openapi.yml
- filename: payu-mcp-api-openapi.yml
  format: yaml
  label: PayU MCP API
  slug: payu-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-mcp-api-openapi.yml
- filename: payu-order-api-openapi.yml
  format: yaml
  label: PayU Order API
  slug: payu-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-order-api-openapi.yml
- filename: payu-partner-merchant-registration-api-openapi.yml
  format: yaml
  label: PayU Partner-Merchant-Registration API
  slug: payu-partner-merchant-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-partner-merchant-registration-api-openapi.yml
- filename: payu-payment-methods-api-openapi.yml
  format: yaml
  label: PayU Payment-Methods API
  slug: payu-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-payment-methods-api-openapi.yml
- filename: payu-payout-api-openapi.yml
  format: yaml
  label: PayU Payout API
  slug: payu-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-payout-api-openapi.yml
- filename: payu-pf-submerchant-registration-api-openapi.yml
  format: yaml
  label: PayU PF-Submerchant-Registration API
  slug: payu-pf-submerchant-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-pf-submerchant-registration-api-openapi.yml
- filename: payu-refund-api-openapi.yml
  format: yaml
  label: PayU Refund API
  slug: payu-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-refund-api-openapi.yml
- filename: payu-shop-api-openapi.yml
  format: yaml
  label: PayU Shop API
  slug: payu-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-shop-api-openapi.yml
- filename: payu-statements-api-openapi.yml
  format: yaml
  label: PayU Statements API
  slug: payu-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-statements-api-openapi.yml
- filename: payu-token-api-openapi.yml
  format: yaml
  label: PayU Token API
  slug: payu-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payu.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: corporate.payu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: developers.payu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: secure.payu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayU, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PayU
provider_slug: payu
slug: payu-domain-security
source_filename: payu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.payu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.payu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: secure.payu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: payu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/security/payu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Fintech
- Financial Services
- Subscriptions
- Fraud Detection
- Checkout
- Marketplace
- Tokenization
- Emerging Markets
---
