---
api_key_in:
- header
api_specs:
- filename: pinwheel-accounts-api-openapi.yml
  format: yaml
  label: Pinwheel Accounts API
  slug: pinwheel-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-accounts-api-openapi.yml
- filename: pinwheel-api-keys-api-openapi.yml
  format: yaml
  label: Pinwheel API Keys API
  slug: pinwheel-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-api-keys-api-openapi.yml
- filename: pinwheel-company-connect-api-openapi.yml
  format: yaml
  label: Pinwheel Company Connect API
  slug: pinwheel-company-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-company-connect-api-openapi.yml
- filename: pinwheel-direct-deposit-allocations-api-openapi.yml
  format: yaml
  label: Pinwheel Direct Deposit Allocations API
  slug: pinwheel-direct-deposit-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-direct-deposit-allocations-api-openapi.yml
- filename: pinwheel-earnings-stream-api-openapi.yml
  format: yaml
  label: Pinwheel Earnings Stream API
  slug: pinwheel-earnings-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-earnings-stream-api-openapi.yml
- filename: pinwheel-employers-and-platforms-api-openapi.yml
  format: yaml
  label: Pinwheel Employers and Platforms API
  slug: pinwheel-employers-and-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-employers-and-platforms-api-openapi.yml
- filename: pinwheel-end-users-api-openapi.yml
  format: yaml
  label: Pinwheel End Users API
  slug: pinwheel-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-end-users-api-openapi.yml
- filename: pinwheel-income-and-employment-api-openapi.yml
  format: yaml
  label: Pinwheel Income and Employment API
  slug: pinwheel-income-and-employment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-income-and-employment-api-openapi.yml
- filename: pinwheel-jobs-api-openapi.yml
  format: yaml
  label: Pinwheel Jobs API
  slug: pinwheel-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-jobs-api-openapi.yml
- filename: pinwheel-link-tokens-api-openapi.yml
  format: yaml
  label: Pinwheel Link Tokens API
  slug: pinwheel-link-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-link-tokens-api-openapi.yml
- filename: pinwheel-sandbox-api-openapi.yml
  format: yaml
  label: Pinwheel Sandbox API
  slug: pinwheel-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-sandbox-api-openapi.yml
- filename: pinwheel-tax-forms-api-openapi.yml
  format: yaml
  label: Pinwheel Tax Forms API
  slug: pinwheel-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-tax-forms-api-openapi.yml
- filename: pinwheel-verification-reports-api-openapi.yml
  format: yaml
  label: Pinwheel Verification Reports API
  slug: pinwheel-verification-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-verification-reports-api-openapi.yml
- filename: pinwheel-webhooks-api-openapi.yml
  format: yaml
  label: Pinwheel Webhooks API
  slug: pinwheel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/openapi/pinwheel-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pinwheel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinwheel secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pinwheel
provider_slug: pinwheel
scheme_count: 2
schemes:
- description: API Secret
  in: header
  name: apiSecret
  parameter: X-API-SECRET
  sources:
  - openapi/pinwheel-pinwheel-api-openapi.yml
  type: apiKey
- description: Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pinwheel-pinwheel-api-openapi.yml
  type: http
slug: pinwheel-authentication
source_filename: pinwheel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pinwheel-pinwheel-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiSecret\n  type: apiKey\n  in: header\n  parameter: X-API-SECRET\n  description: API Secret\n  sources:\n  - openapi/pinwheel-pinwheel-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token\n  sources:\n  - openapi/pinwheel-pinwheel-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinwheel/refs/heads/main/authentication/pinwheel-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payroll
- Direct Deposit
- Income Verification
- Employment
- Tax Forms
- Fintech
- Open Finance
- Bill Switching
- Financial Data
---
