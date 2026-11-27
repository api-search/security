---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xplor-pay-openapi-generated.yml
  format: yaml
  label: Xplor Pay API
  slug: xplor-pay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xplor-pay/openapi/_ae-authored/xplor-pay-openapi-generated.yml
auth_types: []
description: Authentication methods documented for Xplor Pay
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Xplor Pay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xplor Pay declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Xplor Pay
provider_slug: xplor-pay
scheme_count: 2
schemes:
- evidence: When a secret is configured, Xplor Pay includes it in the `X-Webhook-Secret` HTTP request header.
  header: X-Webhook-Secret
  how_to_obtain: Generate a secret, store it securely, and share it with Xplor Pay Support to have it configured for your webhook.
  location: header
  name: Shared-secret
  type: other
- evidence: An access API key issued to you by Xplor Pay.
  header: api-key
  how_to_obtain: Issued by Xplor Pay to the merchant.
  location: header
  name: API Key
  type: apiKey
slug: xplor-pay-authentication
source_filename: xplor-pay-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.xplorpay.com/api-reference/webhooks/webhook-authentication.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.xplorpay.com/api-reference/webhooks/webhook-authentication.md\nsources:\n- https://docs.xplorpay.com/api-reference/webhooks/webhook-authentication.md\n- https://docs.xplorpay.com/guides/mobile-emv/generate-json-web-token.md\n- https://docs.xplorpay.com/api-reference/api/payments/cards-card-not-present/vault/tokens.md\n- https://docs.xplorpay.com/api-reference/api/payments/ach/ach-vault-token.md\ndescription: Authentication methods documented for Xplor Pay\nschemes:\n- type: other\n  name: Shared-secret\n  evidence: When a secret is configured, Xplor Pay includes it in the `X-Webhook-Secret` HTTP request header.\n  location: header\n  header: X-Webhook-Secret\n  how_to_obtain: Generate a secret, store it securely, and share it with Xplor Pay Support to have it configured for your webhook.\n- type: apiKey\n  name: API Key\n  evidence: An access API key issued to you by\
  \ Xplor Pay.\n  location: header\n  header: api-key\n  how_to_obtain: Issued by Xplor Pay to the merchant.\ndocs: https://docs.xplorpay.com/api-reference/webhooks/webhook-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/xplor-pay/authentication/xplor-pay-authentication.yml
summary_line: 2 schemes
tags:
- Embedded Payments
- PayFac as a Service
- Merchant Solutions
- Vertical SaaS
---
