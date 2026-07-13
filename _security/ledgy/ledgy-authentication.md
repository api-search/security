---
api_key_in: []
api_specs:
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Companies API
  slug: companies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Stakeholders API
  slug: stakeholders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Share Classes API
  slug: share-classes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Financing Rounds API
  slug: financing-rounds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy ESOP and Grants API
  slug: esop-grants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ledgy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ledgy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ledgy
provider_slug: ledgy
scheme_count: 1
schemes:
- description: Company API key sent as a Bearer token. Reveal it from your company's general settings page in the Ledgy app.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ledgy-openapi.yml
  type: http
slug: ledgy-authentication
source_filename: ledgy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ledgy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Company API key sent as a Bearer token. Reveal it from your company's general\n    settings page in the Ledgy app.\n  sources:\n  - openapi/ledgy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/authentication/ledgy-authentication.yml
summary_line: http · 1 scheme
tags:
- Equity Management
- Cap Table
- ESOP
- Stakeholders
- GraphQL
---
