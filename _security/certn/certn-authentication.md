---
api_key_in: []
api_specs:
- filename: certn-openapi.yml
  format: yaml
  label: Certn Applications API
  slug: certn-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Checks API
  slug: certn-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Reports API
  slug: certn-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Packages API
  slug: certn-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Webhooks API
  slug: certn-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Teams and Users API
  slug: certn-teams-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Certn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Certn secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Certn
provider_slug: certn
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 client credentials. Exchange your Client ID and Client Secret for an access token, then send it as "Authorization: Bearer {token}".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/certn-openapi.yml
  type: http
slug: certn-authentication
source_filename: certn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/certn-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth 2.0 client credentials. Exchange your Client ID and Client Secret for\n    an access token, then send it as \"Authorization: Bearer {token}\".'\n  sources:\n  - openapi/certn-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/authentication/certn-authentication.yml
summary_line: http · 1 scheme
tags:
- Background Checks
- Identity Verification
- Criminal Record Check
- Screening
- HR Tech
- Compliance
- Trust and Safety
---
