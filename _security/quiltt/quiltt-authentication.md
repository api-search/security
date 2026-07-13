---
api_key_in: []
api_specs:
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Profiles API
  slug: quiltt-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Connections API
  slug: quiltt-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Session Tokens API
  slug: quiltt-session-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Webhooks API
  slug: quiltt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quiltt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quiltt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quiltt
provider_slug: quiltt
scheme_count: 1
schemes:
- description: Your Quiltt API Secret Key used for Admin and token-issuance calls.
  name: apiSecretKey
  scheme: bearer
  sources:
  - openapi/quiltt-openapi.yml
  type: http
slug: quiltt-authentication
source_filename: quiltt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quiltt-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiSecretKey\n  type: http\n  scheme: bearer\n  description: Your Quiltt API Secret Key used for Admin and token-issuance calls.\n  sources:\n  - openapi/quiltt-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/authentication/quiltt-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Open Banking
- Financial Data
- Aggregation
- GraphQL
---
