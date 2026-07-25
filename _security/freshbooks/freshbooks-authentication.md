---
api_key_in: []
api_specs:
- filename: start
  format: yaml
  label: FreshBooks REST API
  slug: freshbooks-api
  spec_type: Postman
  url: https://www.freshbooks.com/api/start
- filename: freshbooks-webhooks-asyncapi.yml
  format: yaml
  label: FreshBooks Webhooks (Callbacks API)
  slug: freshbooks-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/asyncapi/freshbooks-webhooks-asyncapi.yml
- filename: freshbooks-auth-api-openapi.yml
  format: yaml
  label: FreshBooks Auth API
  slug: freshbooks-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-auth-api-openapi.yml
- filename: freshbooks-clients-api-openapi.yml
  format: yaml
  label: FreshBooks Clients API
  slug: freshbooks-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-clients-api-openapi.yml
- filename: freshbooks-estimates-api-openapi.yml
  format: yaml
  label: FreshBooks Estimates API
  slug: freshbooks-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-estimates-api-openapi.yml
- filename: freshbooks-expenses-api-openapi.yml
  format: yaml
  label: FreshBooks Expenses API
  slug: freshbooks-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-expenses-api-openapi.yml
- filename: freshbooks-invoices-api-openapi.yml
  format: yaml
  label: FreshBooks Invoices API
  slug: freshbooks-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-invoices-api-openapi.yml
- filename: freshbooks-items-api-openapi.yml
  format: yaml
  label: FreshBooks Items API
  slug: freshbooks-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-items-api-openapi.yml
- filename: freshbooks-payments-api-openapi.yml
  format: yaml
  label: FreshBooks Payments API
  slug: freshbooks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-payments-api-openapi.yml
- filename: freshbooks-projects-api-openapi.yml
  format: yaml
  label: FreshBooks Projects API
  slug: freshbooks-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-projects-api-openapi.yml
- filename: freshbooks-tasks-api-openapi.yml
  format: yaml
  label: FreshBooks Tasks API
  slug: freshbooks-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-tasks-api-openapi.yml
- filename: freshbooks-taxes-api-openapi.yml
  format: yaml
  label: FreshBooks Taxes API
  slug: freshbooks-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-taxes-api-openapi.yml
- filename: freshbooks-timeentries-api-openapi.yml
  format: yaml
  label: FreshBooks TimeEntries API
  slug: freshbooks-timeentries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-timeentries-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freshbooks Authentication
name_suffix: Authentication
oauth_flows: []
overview: FreshBooks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FreshBooks
provider_slug: freshbooks
scheme_count: 1
schemes:
- description: OAuth 2.0 access token obtained via the FreshBooks authorization code flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freshbooks-openapi.yml
  type: http
slug: freshbooks-authentication
source_filename: freshbooks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshbooks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token obtained via the FreshBooks authorization code flow.\n  sources:\n  - openapi/freshbooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/authentication/freshbooks-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Invoicing
- Expense Tracking
- Time Tracking
- Small Business
- Bookkeeping
---
