---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: open-financial-accounts-api-openapi.yml
  format: yaml
  label: Open (open.money) Accounts API
  slug: open-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-accounts-api-openapi.yml
- filename: open-financial-constants-api-openapi.yml
  format: yaml
  label: Open (open.money) Constants API
  slug: open-financial-constants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-constants-api-openapi.yml
- filename: open-financial-events-api-openapi.yml
  format: yaml
  label: Open (open.money) Events API
  slug: open-financial-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-events-api-openapi.yml
- filename: open-financial-icp-api-openapi.yml
  format: yaml
  label: Open (open.money) Icp API
  slug: open-financial-icp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-icp-api-openapi.yml
- filename: open-financial-kycs-api-openapi.yml
  format: yaml
  label: Open (open.money) Kycs API
  slug: open-financial-kycs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-kycs-api-openapi.yml
- filename: open-financial-pg-api-openapi.yml
  format: yaml
  label: Open (open.money) Pg API
  slug: open-financial-pg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-pg-api-openapi.yml
- filename: open-financial-pg-settlements-api-openapi.yml
  format: yaml
  label: Open (open.money) Pg Settlements API
  slug: open-financial-pg-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-pg-settlements-api-openapi.yml
- filename: open-financial-refund-api-openapi.yml
  format: yaml
  label: Open (open.money) Refund API
  slug: open-financial-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-refund-api-openapi.yml
- filename: open-financial-transfers-api-openapi.yml
  format: yaml
  label: Open (open.money) Transfers API
  slug: open-financial-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-transfers-api-openapi.yml
- filename: open-financial-verifications-api-openapi.yml
  format: yaml
  label: Open (open.money) Verifications API
  slug: open-financial-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-verifications-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Open Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open (open.money) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open (open.money)
provider_slug: open-financial
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/open-financial-1-openapi.yml
  - openapi/open-financial-2-openapi.yml
  - openapi/open-financial-4-openapi.yml
  - openapi/open-financial-5-openapi.yml
  - openapi/open-financial-6-openapi.yml
  - openapi/open-financial-8-openapi.yml
  type: apiKey
slug: open-financial-authentication
source_filename: open-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/open-financial-1-openapi.yml, openapi/open-financial-2-openapi.yml, openapi/open-financial-4-openapi.yml,\n  openapi/open-financial-5-openapi.yml, openapi/open-financial-6-openapi.yml, openapi/open-financial-8-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/open-financial-1-openapi.yml\n  - openapi/open-financial-2-openapi.yml\n  - openapi/open-financial-4-openapi.yml\n  - openapi/open-financial-5-openapi.yml\n  - openapi/open-financial-6-openapi.yml\n  - openapi/open-financial-8-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/authentication/open-financial-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Connected Banking
- Neobank
- Small Business
- Embedded Finance
- Banking as a Service
- Payments
- Payouts
- UPI
- Accounting
- Payroll
- Expense Management
- India
- Fintech
---
