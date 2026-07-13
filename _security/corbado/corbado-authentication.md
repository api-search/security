---
api_key_in: []
api_specs:
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Users API
  slug: corbado-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Identifiers API
  slug: corbado-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Sessions API
  slug: corbado-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Passkeys API
  slug: corbado-passkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Connect Tokens API
  slug: corbado-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Projects API
  slug: corbado-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Corbado Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corbado secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Corbado
provider_slug: corbado
scheme_count: 1
schemes:
- description: HTTP Basic authentication. The username is the project ID (e.g. pro-1234567890) and the password is the API secret, both issued from the Corbado Developer Panel.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/corbado-openapi.yml
  type: http
slug: corbado-authentication
source_filename: corbado-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/corbado-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. The username is the project ID (e.g. pro-1234567890)\n    and the password is the API secret, both issued from the Corbado Developer Panel.\n  sources:\n  - openapi/corbado-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/authentication/corbado-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Passkeys
- WebAuthn
- Passwordless
- CIAM
- Identity
---
