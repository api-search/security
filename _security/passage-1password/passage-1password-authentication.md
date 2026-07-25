---
api_key_in: []
api_specs:
- filename: passage-1password-devices-api-openapi.yml
  format: yaml
  label: Passage by 1Password Devices API
  slug: passage-1password-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-devices-api-openapi.yml
- filename: passage-1password-magic-links-api-openapi.yml
  format: yaml
  label: Passage by 1Password Magic Links API
  slug: passage-1password-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-magic-links-api-openapi.yml
- filename: passage-1password-tokens-api-openapi.yml
  format: yaml
  label: Passage by 1Password Tokens API
  slug: passage-1password-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-tokens-api-openapi.yml
- filename: passage-1password-users-api-openapi.yml
  format: yaml
  label: Passage by 1Password Users API
  slug: passage-1password-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Passage 1Password Authentication
name_suffix: Authentication
oauth_flows: []
overview: Passage by 1Password secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Passage by 1Password
provider_slug: passage-1password
scheme_count: 1
schemes:
- description: 'Passage Management API key, sent as: Authorization: Bearer <PASSAGE_API_KEY>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/passage-1password-openapi.yml
  type: http
slug: passage-1password-authentication
source_filename: passage-1password-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/passage-1password-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Passage Management API key, sent as: Authorization: Bearer <PASSAGE_API_KEY>'\n  sources:\n  - openapi/passage-1password-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/authentication/passage-1password-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Passkeys
- WebAuthn
- Passwordless
- Identity
- Magic Links
---
