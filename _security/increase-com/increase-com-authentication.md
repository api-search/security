---
api_key_in: []
api_specs:
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Accounts API
  slug: increase-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Account Numbers API
  slug: increase-com-account-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Cards API
  slug: increase-com-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Card Payments API
  slug: increase-com-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase ACH Transfers API
  slug: increase-com-ach-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Wire Transfers API
  slug: increase-com-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Real-Time Payments API
  slug: increase-com-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Checks API
  slug: increase-com-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Transactions API
  slug: increase-com-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Entities API
  slug: increase-com-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Events and Webhooks API
  slug: increase-com-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Bookkeeping API
  slug: increase-com-bookkeeping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Card Profiles and Digital Wallets API
  slug: increase-com-card-profiles-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Lockboxes API
  slug: increase-com-lockboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Simulations API
  slug: increase-com-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Increase Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Increase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Increase
provider_slug: increase-com
scheme_count: 1
schemes:
- description: 'Increase API key passed as `Authorization: Bearer YOUR_API_KEY`. Keys are environment-scoped (production vs sandbox). OAuth is also supported for platform / Increase-for-platforms integrations.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/increase-com-openapi.yml
  type: http
slug: increase-com-authentication
source_filename: increase-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/increase-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Increase API key passed as `Authorization: Bearer YOUR_API_KEY`. Keys are environment-scoped\n    (production vs sandbox). OAuth is also supported for platform / Increase-for-platforms integrations.'\n  sources:\n  - openapi/increase-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/authentication/increase-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Banking
- Financial Infrastructure
- ACH
- Wire Transfers
- Real-Time Payments
- Cards
- Fintech
---
