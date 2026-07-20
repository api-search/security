---
api_specs:
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Charges API
  slug: payjp-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Customers API
  slug: payjp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Cards API
  slug: payjp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Tokens API
  slug: payjp-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Plans API
  slug: payjp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Subscriptions API
  slug: payjp-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Transfers API
  slug: payjp-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Statements & Balances API
  slug: payjp-statements-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Events & Webhooks API
  slug: payjp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP 3D Secure API
  slug: payjp-three-d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Platform API (Tenants)
  slug: payjp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Account API
  slug: payjp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
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
- FinTech
- Japan
- Credit Cards
- Subscriptions
- Tokenization
trust_url: https://pay.jp/
---
