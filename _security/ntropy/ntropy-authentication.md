---
api_key_in:
- header
api_specs:
- filename: ntropy-api-v3-openapi-original.json
  format: json
  label: Ntropy Transaction API (v3)
  slug: ntropy-transaction-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-api-v3-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ntropy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ntropy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ntropy
provider_slug: ntropy
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/ntropy-api-v3-openapi-original.json
  - openapi/ntropy-transaction-api-openapi-original.json
  type: apiKey
slug: ntropy-authentication
source_filename: ntropy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/ntropy-api-v3-openapi-original.json, openapi/ntropy-transaction-api-openapi-original.json\ndocs: https://docs.ntropy.com/api/auth\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Single auth mechanism: an API key sent in the X-API-KEY request header. Keys are\n    created, disabled and rotated in the dashboard (https://dashboard.ntropy.com/keys).\n    Rotating a key changes only its authorization; previously submitted data stays\n    accessible. No OAuth/OIDC.\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ntropy-api-v3-openapi-original.json\n  - openapi/ntropy-transaction-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/authentication/ntropy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Transaction Enrichment
- Financial Data
- Data Enrichment
- Bank Statements
- Categorization
- Underwriting
---
