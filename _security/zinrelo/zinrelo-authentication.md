---
api_key_in:
- header
api_specs:
- filename: zinrelo-events-api-openapi.yml
  format: yaml
  label: Zinrelo Events API
  slug: zinrelo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-events-api-openapi.yml
- filename: zinrelo-members-api-openapi.yml
  format: yaml
  label: Zinrelo Members API
  slug: zinrelo-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-members-api-openapi.yml
- filename: zinrelo-points-api-openapi.yml
  format: yaml
  label: Zinrelo Points API
  slug: zinrelo-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-points-api-openapi.yml
- filename: zinrelo-redemptions-api-openapi.yml
  format: yaml
  label: Zinrelo Redemptions API
  slug: zinrelo-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-redemptions-api-openapi.yml
- filename: zinrelo-rewards-api-openapi.yml
  format: yaml
  label: Zinrelo Rewards API
  slug: zinrelo-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-rewards-api-openapi.yml
- filename: zinrelo-tiers-api-openapi.yml
  format: yaml
  label: Zinrelo Tiers API
  slug: zinrelo-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-tiers-api-openapi.yml
- filename: zinrelo-transactions-api-openapi.yml
  format: yaml
  label: Zinrelo Transactions API
  slug: zinrelo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zinrelo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zinrelo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zinrelo
provider_slug: zinrelo
scheme_count: 2
schemes:
- description: Your Zinrelo Partner ID, provisioned to your account.
  in: header
  name: partnerId
  parameter: partner-id
  sources:
  - openapi/zinrelo-openapi.yml
  type: apiKey
- description: Your Zinrelo API key, provisioned to your account.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/zinrelo-openapi.yml
  type: apiKey
slug: zinrelo-authentication
source_filename: zinrelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zinrelo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: partnerId\n  type: apiKey\n  in: header\n  parameter: partner-id\n  description: Your Zinrelo Partner ID, provisioned to your account.\n  sources:\n  - openapi/zinrelo-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Your Zinrelo API key, provisioned to your account.\n  sources:\n  - openapi/zinrelo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/authentication/zinrelo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Loyalty
- Rewards
- Points
- Customer Retention
- E-Commerce
- Software-as-a-Service
---
