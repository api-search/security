---
api_key_in:
- header
api_specs:
- filename: recharge-payments-openapi.yml
  format: yaml
  label: Recharge Subscriptions API
  slug: recharge-payments-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-openapi.yml
- filename: recharge-payments-openapi.yml
  format: yaml
  label: Recharge Customers API
  slug: recharge-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-openapi.yml
- filename: recharge-payments-openapi.yml
  format: yaml
  label: Recharge Orders API
  slug: recharge-payments-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-openapi.yml
- filename: recharge-payments-openapi.yml
  format: yaml
  label: Recharge Charges API
  slug: recharge-payments-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-openapi.yml
- filename: recharge-payments-openapi.yml
  format: yaml
  label: Recharge Products API
  slug: recharge-payments-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-openapi.yml
- filename: recharge-payments-openapi.yml
  format: yaml
  label: Recharge Webhooks API
  slug: recharge-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Recharge Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recharge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Recharge
provider_slug: recharge-payments
scheme_count: 1
schemes:
- description: Store API token generated in the Recharge merchant portal under Apps and integrations.
  in: header
  name: apiToken
  parameter: X-Recharge-Access-Token
  sources:
  - openapi/recharge-payments-openapi.yml
  type: apiKey
slug: recharge-payments-authentication
source_filename: recharge-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/recharge-payments-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: X-Recharge-Access-Token\n  description: Store API token generated in the Recharge merchant portal under Apps and integrations.\n  sources:\n  - openapi/recharge-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/authentication/recharge-payments-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Subscriptions
- Recurring Billing
- E-commerce
- Payments
- Shopify
- Retention
---
