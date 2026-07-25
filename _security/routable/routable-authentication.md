---
api_key_in: []
api_specs:
- filename: routable-companies-api-openapi.yml
  format: yaml
  label: Routable Companies API
  slug: routable-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-companies-api-openapi.yml
- filename: routable-contacts-api-openapi.yml
  format: yaml
  label: Routable Contacts API
  slug: routable-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-contacts-api-openapi.yml
- filename: routable-funding-sources-api-openapi.yml
  format: yaml
  label: Routable Funding Sources API
  slug: routable-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-funding-sources-api-openapi.yml
- filename: routable-payables-api-openapi.yml
  format: yaml
  label: Routable Payables API
  slug: routable-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-payables-api-openapi.yml
- filename: routable-payment-methods-api-openapi.yml
  format: yaml
  label: Routable Payment Methods API
  slug: routable-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-payment-methods-api-openapi.yml
- filename: routable-receivables-api-openapi.yml
  format: yaml
  label: Routable Receivables API
  slug: routable-receivables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-receivables-api-openapi.yml
- filename: routable-webhooks-api-openapi.yml
  format: yaml
  label: Routable Webhooks API
  slug: routable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-webhooks-api-openapi.yml
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
