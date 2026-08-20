---
api_key_in:
- header
api_specs:
- filename: stigg-coupons-api-openapi.yml
  format: yaml
  label: Stigg Coupons API
  slug: stigg-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-coupons-api-openapi.yml
- filename: stigg-customers-api-openapi.yml
  format: yaml
  label: Stigg Customers API
  slug: stigg-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-customers-api-openapi.yml
- filename: stigg-entitlements-api-openapi.yml
  format: yaml
  label: Stigg Entitlements API
  slug: stigg-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-entitlements-api-openapi.yml
- filename: stigg-subscriptions-api-openapi.yml
  format: yaml
  label: Stigg Subscriptions API
  slug: stigg-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-subscriptions-api-openapi.yml
- filename: stigg-usage-api-openapi.yml
  format: yaml
  label: Stigg Usage API
  slug: stigg-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stigg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stigg secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stigg
provider_slug: stigg
scheme_count: 1
schemes:
- description: Full access key from the Stigg dashboard (Integrations > API keys).
  in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/stigg-openapi.yml
  - openapi/stigg-rest-openapi.yml
  type: apiKey
slug: stigg-authentication
source_filename: stigg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stigg-openapi.yml, openapi/stigg-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Full access key from the Stigg dashboard (Integrations > API keys).\n  sources:\n  - openapi/stigg-openapi.yml\n  - openapi/stigg-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/authentication/stigg-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- FinOps
- Pricing
- Billing
- Entitlements
- Usage-Based Billing
- Feature Flags
- Product-Led Growth
- Subscription
- Software-as-a-Service
- GraphQL
- REST
---
