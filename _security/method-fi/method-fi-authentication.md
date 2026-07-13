---
api_key_in: []
api_specs:
- filename: method-fi-openapi.yml
  format: yaml
  label: Method Entities API
  slug: entities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-openapi.yml
- filename: method-fi-openapi.yml
  format: yaml
  label: Method Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-openapi.yml
- filename: method-fi-openapi.yml
  format: yaml
  label: Method Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-openapi.yml
- filename: method-fi-openapi.yml
  format: yaml
  label: Method Merchants API
  slug: merchants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-openapi.yml
- filename: method-fi-openapi.yml
  format: yaml
  label: Method Connect API
  slug: connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-openapi.yml
- filename: method-fi-openapi.yml
  format: yaml
  label: Method Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-openapi.yml
- filename: method-fi-openapi.yml
  format: yaml
  label: Method Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Method Fi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Method Financial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Method Financial
provider_slug: method-fi
scheme_count: 1
schemes:
- description: Provide your Method API key as a Bearer token in the Authorization header. Optionally send a Method-Version header (e.g. 2026-03-30).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/method-fi-openapi.yml
  type: http
slug: method-fi-authentication
source_filename: method-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/method-fi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Provide your Method API key as a Bearer token in the Authorization header. Optionally\n    send a Method-Version header (e.g. 2026-03-30).\n  sources:\n  - openapi/method-fi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/authentication/method-fi-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- Payments
- Liabilities
- Debt
- Embedded Finance
---
