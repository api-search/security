---
api_key_in: []
api_specs:
- filename: persona-accounts-api-openapi.yml
  format: yaml
  label: Persona Accounts API
  slug: persona-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-accounts-api-openapi.yml
- filename: persona-inquiries-api-openapi.yml
  format: yaml
  label: Persona Inquiries API
  slug: persona-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-inquiries-api-openapi.yml
- filename: persona-lists-api-openapi.yml
  format: yaml
  label: Persona Lists API
  slug: persona-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-lists-api-openapi.yml
- filename: persona-reports-api-openapi.yml
  format: yaml
  label: Persona Reports API
  slug: persona-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-reports-api-openapi.yml
- filename: persona-transactions-api-openapi.yml
  format: yaml
  label: Persona Transactions API
  slug: persona-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-transactions-api-openapi.yml
- filename: persona-verifications-api-openapi.yml
  format: yaml
  label: Persona Verifications API
  slug: persona-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-verifications-api-openapi.yml
- filename: persona-webhooks-api-openapi.yml
  format: yaml
  label: Persona Webhooks API
  slug: persona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Persona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Persona secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Persona
provider_slug: persona
scheme_count: 1
schemes:
- description: 'Persona uses bearer-token authentication. Pass your API key as

    `Authorization: Bearer <YOUR_API_KEY>` on every request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/persona-openapi.yml
  type: http
slug: persona-authentication
source_filename: persona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/persona-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Persona uses bearer-token authentication. Pass your API key as\n    `Authorization: Bearer <YOUR_API_KEY>` on every request.\n  sources:\n  - openapi/persona-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/authentication/persona-authentication.yml
summary_line: http · 1 scheme
tags:
- Fraud Prevention
- Identity Verification
- KYC
---
