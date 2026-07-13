---
api_key_in:
- header
api_specs:
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Access Tokens API
  slug: atomic-fi-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Transact SDK
  slug: atomic-fi-transact-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Tasks API
  slug: atomic-fi-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Deposit API
  slug: atomic-fi-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Verify API
  slug: atomic-fi-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic PayLink API
  slug: atomic-fi-paylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Data & Transactions API
  slug: atomic-fi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Webhooks API
  slug: atomic-fi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Atomic Fi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atomic secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Atomic
provider_slug: atomic-fi
scheme_count: 2
schemes:
- description: API Key sent in the x-api-key header, paired with the x-api-secret header. Used for backend-to-backend calls.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/atomic-fi-openapi.yml
  type: apiKey
- description: Public token for permitted client-side requests.
  in: header
  name: PublicTokenAuth
  parameter: x-public-token
  sources:
  - openapi/atomic-fi-openapi.yml
  type: apiKey
slug: atomic-fi-authentication
source_filename: atomic-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atomic-fi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Key sent in the x-api-key header, paired with the x-api-secret header. Used\n    for backend-to-backend calls.\n  sources:\n  - openapi/atomic-fi-openapi.yml\n- name: PublicTokenAuth\n  type: apiKey\n  in: header\n  parameter: x-public-token\n  description: Public token for permitted client-side requests.\n  sources:\n  - openapi/atomic-fi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/authentication/atomic-fi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Fintech
- Payroll
- Direct Deposit
- Income Verification
- Employment Verification
- Financial Connectivity
- Embedded Finance
---
