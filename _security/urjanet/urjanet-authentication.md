---
api_key_in: []
api_specs:
- filename: urjanet-authentication-api-openapi.yml
  format: yaml
  label: Urjanet Authentication API
  slug: urjanet-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-authentication-api-openapi.yml
- filename: urjanet-credentials-connections-api-openapi.yml
  format: yaml
  label: Urjanet Credentials & Connections API
  slug: urjanet-credentials-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-credentials-connections-api-openapi.yml
- filename: urjanet-meters-api-openapi.yml
  format: yaml
  label: Urjanet Meters API
  slug: urjanet-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-meters-api-openapi.yml
- filename: urjanet-statements-bills-api-openapi.yml
  format: yaml
  label: Urjanet Statements & Bills API
  slug: urjanet-statements-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-statements-bills-api-openapi.yml
- filename: urjanet-users-api-openapi.yml
  format: yaml
  label: Urjanet Users API
  slug: urjanet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-users-api-openapi.yml
- filename: urjanet-webhooks-api-openapi.yml
  format: yaml
  label: Urjanet Webhooks API
  slug: urjanet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Urjanet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Urjanet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Urjanet
provider_slug: urjanet
scheme_count: 1
schemes:
- description: Bearer token obtained from POST /auth/login, sent in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/urjanet-openapi.yml
  type: http
slug: urjanet-authentication
source_filename: urjanet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/urjanet-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from POST /auth/login, sent in the Authorization header\n    as \"Bearer {token}\".\n  sources:\n  - openapi/urjanet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/authentication/urjanet-authentication.yml
summary_line: http · 1 scheme
tags:
- Utility Data
- Energy
- Utility Bills
- Aggregation
- Meters
- Sustainability
---
