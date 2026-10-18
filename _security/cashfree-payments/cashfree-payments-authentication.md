---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cashfree-payments-orders-api-openapi.yml
  format: yaml
  label: Cashfree Payments Orders API
  slug: cashfree-payments-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree-payments/refs/heads/main/openapi/cashfree-payments-orders-api-openapi.yml
- filename: cashfree-payments-payout-api-openapi.yml
  format: yaml
  label: Cashfree Payments Payout API
  slug: cashfree-payments-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree-payments/refs/heads/main/openapi/cashfree-payments-payout-api-openapi.yml
- filename: cashfree-payments-pg-api-openapi.yml
  format: yaml
  label: Cashfree Payments Pg API
  slug: cashfree-payments-pg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree-payments/refs/heads/main/openapi/cashfree-payments-pg-api-openapi.yml
auth_types: []
description: Cashfree uses API key based authentication via custom headers.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cashfree Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cashfree Payments declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Cashfree Payments
provider_slug: cashfree-payments
scheme_count: 4
schemes:
- evidence: The standard authentication for merchants uses two specific headers x-client-id and x-client-secret . Pass your appId and secretKey in these fields.
  header: x-client-id
  how_to_obtain: Generate API keys in the Payment Gateway Dashboard under Developers → API Keys.
  location: header
  name: Merchant authentication
  type: apiKey
- evidence: The standard authentication for merchants uses two specific headers x-client-id and x-client-secret . Pass your appId and secretKey in these fields.
  header: x-client-secret
  how_to_obtain: Generate API keys in the Payment Gateway Dashboard under Developers → API Keys.
  location: header
  name: Merchant secret
  type: apiKey
- evidence: You should use the x-partner-apikey and x-partner-merchantid headers instead of the x-client-id and x-client-secret headers.
  header: x-partner-apikey
  how_to_obtain: Generate partner authentication keys via the Partner Dashboard.
  location: header
  name: Partner authentication
  type: apiKey
- evidence: You should use the x-partner-apikey and x-partner-merchantid headers instead of the x-client-id and x-client-secret headers.
  header: x-partner-merchantid
  how_to_obtain: Obtain the merchant ID from the Partner Dashboard > Merchants section.
  location: header
  name: Partner merchant ID
  type: apiKey
slug: cashfree-payments-authentication
source_filename: cashfree-payments-authentication.yml
source_heading: Authentication Profile
source_url: https://www.cashfree.com/docs/api-reference/authentication
source_yaml: "generated: '2026-10-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.cashfree.com/docs/api-reference/authentication\nsources:\n- https://www.cashfree.com/docs/api-reference/authentication\n- https://www.cashfree.com/one-click-onboarding/\n- https://www.cashfree.com/docs/payments/quickstart-guide\n- https://www.cashfree.com/docs/payouts/payout-protect/overview\ndescription: Cashfree uses API key based authentication via custom headers.\nschemes:\n- type: apiKey\n  name: Merchant authentication\n  evidence: The standard authentication for merchants uses two specific headers x-client-id and x-client-secret . Pass your appId and secretKey\n    in these fields.\n  location: header\n  header: x-client-id\n  how_to_obtain: Generate API keys in the Payment Gateway Dashboard under Developers → API Keys.\n- type: apiKey\n  name: Merchant secret\n  evidence: The standard authentication for merchants uses two specific headers x-client-id and x-client-secret\
  \ . Pass your appId and secretKey\n    in these fields.\n  location: header\n  header: x-client-secret\n  how_to_obtain: Generate API keys in the Payment Gateway Dashboard under Developers → API Keys.\n- type: apiKey\n  name: Partner authentication\n  evidence: You should use the x-partner-apikey and x-partner-merchantid headers instead of the x-client-id and x-client-secret headers.\n  location: header\n  header: x-partner-apikey\n  how_to_obtain: Generate partner authentication keys via the Partner Dashboard.\n- type: apiKey\n  name: Partner merchant ID\n  evidence: You should use the x-partner-apikey and x-partner-merchantid headers instead of the x-client-id and x-client-secret headers.\n  location: header\n  header: x-partner-merchantid\n  how_to_obtain: Obtain the merchant ID from the Partner Dashboard > Merchants section.\nnote: No OAuth2 flows are documented for Cashfree authentication.\ndocs: https://www.cashfree.com/docs/api-reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashfree-payments/refs/heads/main/authentication/cashfree-payments-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Payments
- Fintech
- Gateways
---
