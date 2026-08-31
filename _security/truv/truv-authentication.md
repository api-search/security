---
api_key_in:
- header
api_specs:
- filename: truv-admin-api-openapi.yml
  format: yaml
  label: Truv Admin API
  slug: truv-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-admin-api-openapi.yml
- filename: truv-banking-api-openapi.yml
  format: yaml
  label: Truv Banking API
  slug: truv-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-banking-api-openapi.yml
- filename: truv-bridge-tokens-api-openapi.yml
  format: yaml
  label: Truv Bridge Tokens API
  slug: truv-bridge-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-bridge-tokens-api-openapi.yml
- filename: truv-companies-providers-api-openapi.yml
  format: yaml
  label: Truv Companies & Providers API
  slug: truv-companies-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-companies-providers-api-openapi.yml
- filename: truv-direct-deposit-api-openapi.yml
  format: yaml
  label: Truv Direct Deposit API
  slug: truv-direct-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-direct-deposit-api-openapi.yml
- filename: truv-employment-api-openapi.yml
  format: yaml
  label: Truv Employment API
  slug: truv-employment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-employment-api-openapi.yml
- filename: truv-identity-api-openapi.yml
  format: yaml
  label: Truv Identity API
  slug: truv-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-identity-api-openapi.yml
- filename: truv-income-api-openapi.yml
  format: yaml
  label: Truv Income API
  slug: truv-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-income-api-openapi.yml
- filename: truv-insurance-api-openapi.yml
  format: yaml
  label: Truv Insurance API
  slug: truv-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-insurance-api-openapi.yml
- filename: truv-links-api-openapi.yml
  format: yaml
  label: Truv Links API
  slug: truv-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-links-api-openapi.yml
- filename: truv-orders-api-openapi.yml
  format: yaml
  label: Truv Orders API
  slug: truv-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-orders-api-openapi.yml
- filename: truv-pay-statements-api-openapi.yml
  format: yaml
  label: Truv Pay Statements API
  slug: truv-pay-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-pay-statements-api-openapi.yml
- filename: truv-payroll-shifts-api-openapi.yml
  format: yaml
  label: Truv Payroll & Shifts API
  slug: truv-payroll-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-payroll-shifts-api-openapi.yml
- filename: truv-pll-api-openapi.yml
  format: yaml
  label: Truv PLL API
  slug: truv-pll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-pll-api-openapi.yml
- filename: truv-scoring-api-openapi.yml
  format: yaml
  label: Truv Scoring API
  slug: truv-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-scoring-api-openapi.yml
- filename: truv-tasks-api-openapi.yml
  format: yaml
  label: Truv Tasks API
  slug: truv-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-tasks-api-openapi.yml
- filename: truv-tax-api-openapi.yml
  format: yaml
  label: Truv Tax API
  slug: truv-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-tax-api-openapi.yml
- filename: truv-templates-api-openapi.yml
  format: yaml
  label: Truv Templates API
  slug: truv-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-templates-api-openapi.yml
- filename: truv-users-api-openapi.yml
  format: yaml
  label: Truv Users API
  slug: truv-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-users-api-openapi.yml
- filename: truv-webhooks-api-openapi.yml
  format: yaml
  label: Truv Webhooks API
  slug: truv-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-webhooks-api-openapi.yml
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
