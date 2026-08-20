---
api_specs:
- filename: payjp-3d-secure-api-openapi.yml
  format: yaml
  label: PAY.JP 3D Secure API
  slug: payjp-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-3d-secure-api-openapi.yml
- filename: payjp-account-api-openapi.yml
  format: yaml
  label: PAY.JP Account API
  slug: payjp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-account-api-openapi.yml
- filename: payjp-balances-api-openapi.yml
  format: yaml
  label: PAY.JP Balances API
  slug: payjp-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-balances-api-openapi.yml
- filename: payjp-cards-api-openapi.yml
  format: yaml
  label: PAY.JP Cards API
  slug: payjp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-cards-api-openapi.yml
- filename: payjp-charges-api-openapi.yml
  format: yaml
  label: PAY.JP Charges API
  slug: payjp-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-charges-api-openapi.yml
- filename: payjp-customers-api-openapi.yml
  format: yaml
  label: PAY.JP Customers API
  slug: payjp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-customers-api-openapi.yml
- filename: payjp-events-api-openapi.yml
  format: yaml
  label: PAY.JP Events API
  slug: payjp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-events-api-openapi.yml
- filename: payjp-plans-api-openapi.yml
  format: yaml
  label: PAY.JP Plans API
  slug: payjp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-plans-api-openapi.yml
- filename: payjp-platform-api-openapi.yml
  format: yaml
  label: PAY.JP Platform API
  slug: payjp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-platform-api-openapi.yml
- filename: payjp-statements-api-openapi.yml
  format: yaml
  label: PAY.JP Statements API
  slug: payjp-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-statements-api-openapi.yml
- filename: payjp-subscriptions-api-openapi.yml
  format: yaml
  label: PAY.JP Subscriptions API
  slug: payjp-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-subscriptions-api-openapi.yml
- filename: payjp-terms-api-openapi.yml
  format: yaml
  label: PAY.JP Terms API
  slug: payjp-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-terms-api-openapi.yml
- filename: payjp-tokens-api-openapi.yml
  format: yaml
  label: PAY.JP Tokens API
  slug: payjp-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-tokens-api-openapi.yml
- filename: payjp-transfers-api-openapi.yml
  format: yaml
  label: PAY.JP Transfers API
  slug: payjp-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-transfers-api-openapi.yml
certifications:
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Payjp Trust Center
name_suffix: Trust Center
overview: PAY.JP maintains a public trust center documenting PCI DSS compliance.
provider_name: PAY.JP
provider_slug: payjp
slug: payjp-trust-center
source_filename: payjp-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nprobe: true\nsource: https://pay.jp/ and https://help.pay.jp/\nurl: https://pay.jp/\ncertifications:\n- PCI DSS\ncompliance:\n- name: PCI DSS\n  note: >-\n    PAY.JP is built for PCI DSS compliance; card tokenization (payjp.js / Checkout)\n    keeps raw card numbers out of the merchant environment so merchants can qualify\n    for reduced SAQ scope. PAY, Inc. is a registered payment service provider in Japan.\n- name: 3D Secure (EMV 3DS)\n  note: Cardholder authentication supported on charges and stored cards to reduce chargeback/fraud risk.\n- name: Japan (割賦販売法 / Installment Sales Act)\n  note: Operates under Japanese payment/credit regulation as a domestic PSP.\nevidence:\n- source: https://pay.jp/\n  keywords:\n  - PCI DSS\n  - トークン化\n  - 3D Secure\n  - セキュリティ\n- source: https://docs.pay.jp/v1/api/\n  keywords:\n  - 3d_secure\n  - tds_finish\nnotes: >-\n  No dedicated public \"trust center\" portal (e.g. Vanta/SafeBase) was found;\n\
  \  security posture is described across pay.jp and the help center. Verify current\n  certifications directly with PAY, Inc. during reconciliation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/security/payjp-trust-center.yml
summary_line: PCI DSS
tags:
- Payments
- Fintech
- Japan
- Credit Cards
- Subscription
- Tokenization
trust_url: https://pay.jp/
---
