---
api_key_in: []
api_specs:
- filename: routable-openapi.yml
  format: yaml
  label: Routable Vendors API
  slug: vendors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Payables API
  slug: payables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Receivables API
  slug: receivables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Funding Sources API
  slug: funding-sources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Routable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Routable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Routable
provider_slug: routable
scheme_count: 1
schemes:
- description: 'API token presented as `Authorization: Bearer {your_token}`. Generate tokens in the Routable dashboard. A sandbox environment is available for testing without moving real money.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/routable-openapi.yml
  type: http
slug: routable-authentication
source_filename: routable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/routable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token presented as `Authorization: Bearer {your_token}`. Generate tokens\n    in the Routable dashboard. A sandbox environment is available for testing without moving\n    real money.'\n  sources:\n  - openapi/routable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/authentication/routable-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Accounts Payable
- Accounts Receivable
- B2B Payments
- Mass Payouts
- FinTech
---
