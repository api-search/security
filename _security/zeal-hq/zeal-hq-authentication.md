---
api_key_in: []
api_specs:
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Companies API
  slug: zeal-hq-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Employees API
  slug: zeal-hq-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Contractors API
  slug: zeal-hq-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Employee Check (Payroll Run) API
  slug: zeal-hq-employee-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Contractor Payments API
  slug: zeal-hq-contractor-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Pay Schedules API
  slug: zeal-hq-pay-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Worker Onboarding API
  slug: zeal-hq-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Tax and Compliance API
  slug: zeal-hq-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Reports API
  slug: zeal-hq-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Funding and Journal API
  slug: zeal-hq-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Webhooks and Events API
  slug: zeal-hq-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zeal Hq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zeal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zeal
provider_slug: zeal-hq
scheme_count: 1
schemes:
- description: 'Provide your Zeal API key as a Bearer token: `Authorization: Bearer <YOUR_API_KEY>`. Use a test key for Test Mode and a live key for production. Requests are additionally scoped by a companyID passed in the body or query.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zeal-hq-openapi.yml
  type: http
slug: zeal-hq-authentication
source_filename: zeal-hq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeal-hq-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Provide your Zeal API key as a Bearer token: `Authorization: Bearer <YOUR_API_KEY>`.\n    Use a test key for Test Mode and a live key for production. Requests are additionally scoped\n    by a companyID passed in the body or query.'\n  sources:\n  - openapi/zeal-hq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/authentication/zeal-hq-authentication.yml
summary_line: http · 1 scheme
tags:
- Payroll
- Embedded Finance
- Fintech
- Tax Compliance
- Contractors
- Human Resources
---
