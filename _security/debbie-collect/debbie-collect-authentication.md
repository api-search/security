---
api_key_in: []
api_specs:
- filename: debbie-collect-billing-api-openapi.yml
  format: yaml
  label: Debbie Collect Billing API
  slug: debbie-collect-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-billing-api-openapi.yml
- filename: debbie-collect-case-vouchers-api-openapi.yml
  format: yaml
  label: Debbie Collect Case Vouchers API
  slug: debbie-collect-case-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-case-vouchers-api-openapi.yml
- filename: debbie-collect-cases-api-openapi.yml
  format: yaml
  label: Debbie Collect Cases API
  slug: debbie-collect-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-cases-api-openapi.yml
- filename: debbie-collect-creditors-api-openapi.yml
  format: yaml
  label: Debbie Collect Creditors API
  slug: debbie-collect-creditors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-creditors-api-openapi.yml
- filename: debbie-collect-customers-api-openapi.yml
  format: yaml
  label: Debbie Collect Customers API
  slug: debbie-collect-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-customers-api-openapi.yml
- filename: debbie-collect-files-api-openapi.yml
  format: yaml
  label: Debbie Collect Files API
  slug: debbie-collect-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-files-api-openapi.yml
- filename: debbie-collect-payments-api-openapi.yml
  format: yaml
  label: Debbie Collect Payments API
  slug: debbie-collect-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-payments-api-openapi.yml
- filename: debbie-collect-properties-api-openapi.yml
  format: yaml
  label: Debbie Collect Properties API
  slug: debbie-collect-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-properties-api-openapi.yml
- filename: debbie-collect-updates-api-openapi.yml
  format: yaml
  label: Debbie Collect Updates API
  slug: debbie-collect-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-updates-api-openapi.yml
- filename: debbie-collect-webhooks-api-openapi.yml
  format: yaml
  label: Debbie Collect Webhooks API
  slug: debbie-collect-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Debbie Collect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Debbie Collect secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Debbie Collect
provider_slug: debbie-collect
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/debbie-client-api-openapi.yml
  - openapi/debbie-platform-api-openapi.yml
  type: http
slug: debbie-collect-authentication
source_filename: debbie-collect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/debbie-client-api-openapi.yml, openapi/debbie-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/debbie-client-api-openapi.yml\n  - openapi/debbie-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/authentication/debbie-collect-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounts Receivable
- Collection
- Debt Collection
- Fintech
- Payments
- Software-as-a-Service
---
