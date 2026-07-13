---
api_key_in:
- header
api_specs:
- filename: creem-openapi.yml
  format: yaml
  label: Creem Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Checkouts API
  slug: checkouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Discounts API
  slug: discounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Licenses API
  slug: licenses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Creem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creem secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Creem
provider_slug: creem
scheme_count: 1
schemes:
- description: API key for authentication. Find your API key in the Creem dashboard under Developers / Settings > API Keys.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/creem-openapi.yml
  type: apiKey
slug: creem-authentication
source_filename: creem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/creem-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication. Find your API key in the Creem dashboard under Developers\n    / Settings > API Keys.\n  sources:\n  - openapi/creem-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/authentication/creem-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Merchant of Record
- Subscriptions
- SaaS
- Billing
---
