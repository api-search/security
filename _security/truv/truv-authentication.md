---
api_key_in:
- header
api_specs:
- filename: truv-openapi.yml
  format: yaml
  label: Truv Users API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Bridge Tokens API
  slug: bridge-tokens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Links API
  slug: links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Employment Verification API
  slug: employment-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Income Verification API
  slug: income-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Pay Statements API
  slug: pay-statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Direct Deposit Switch API
  slug: direct-deposit-switch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Payroll & Shifts API
  slug: payroll-shifts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Insurance API
  slug: insurance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Identity & Banking API
  slug: identity-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Truv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truv secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Truv
provider_slug: truv
scheme_count: 2
schemes:
- description: Your Truv access client ID.
  in: header
  name: accessClientId
  parameter: X-Access-Client-Id
  sources:
  - openapi/truv-openapi.yml
  type: apiKey
- description: Your Truv access secret.
  in: header
  name: accessSecret
  parameter: X-Access-Secret
  sources:
  - openapi/truv-openapi.yml
  type: apiKey
slug: truv-authentication
source_filename: truv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truv-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessClientId\n  type: apiKey\n  in: header\n  parameter: X-Access-Client-Id\n  description: Your Truv access client ID.\n  sources:\n  - openapi/truv-openapi.yml\n- name: accessSecret\n  type: apiKey\n  in: header\n  parameter: X-Access-Secret\n  description: Your Truv access secret.\n  sources:\n  - openapi/truv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/authentication/truv-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Income Verification
- Employment Verification
- Payroll
- Direct Deposit
- Consumer Permissioned Data
- Fintech
---
