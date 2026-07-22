---
api_key_in:
- header
api_specs:
- filename: spade-openapi-original.yml
  format: yaml
  label: Spade API
  slug: spade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Spade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spade secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spade
provider_slug: spade
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/spade-openapi-original.yml
  type: apiKey
slug: spade-authentication
source_filename: spade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spade-openapi-original.yml\ndocs: https://docs.spade.com/reference/integrate-with-spades-api\nnotes: >-\n  Secret-key auth via the X-Api-Key header, chosen for low-latency applications. Sandbox and\n  production environments use different API keys; keys are issued by a Spade representative.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/spade-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/authentication/spade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Financial Services
- Transaction Enrichment
- Merchant Intelligence
- Payments
- Data Enrichment
- Fraud and Risk
- Fintech
---
