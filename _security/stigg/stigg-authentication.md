---
api_key_in:
- header
api_specs:
- filename: stigg-openapi.yml
  format: yaml
  label: Stigg GraphQL API
  slug: stigg-graphql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-openapi.yml
- filename: stigg-rest-openapi.yml
  format: yaml
  label: Stigg REST API
  slug: stigg-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-rest-openapi.yml
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
- Subscriptions
- SaaS
- GraphQL
- REST
---
