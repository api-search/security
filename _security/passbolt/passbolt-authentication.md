---
api_key_in:
- cookie
api_specs:
- filename: passbolt-openapi.yaml
  format: yaml
  label: Passbolt API
  slug: passbolt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passbolt/refs/heads/main/openapi/passbolt-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Passbolt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Passbolt secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Passbolt
provider_slug: passbolt
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token using a JWT
  name: bearerHttpAuthentication
  scheme: Bearer
  sources:
  - openapi/passbolt-openapi.yaml
  type: http
- description: Session-based authentication. Note that a CSRF token needs to be provided through a header named `X-CSRF-Token`.
  in: cookie
  name: gpgCookieAuthentication
  parameter: passbolt_session
  sources:
  - openapi/passbolt-openapi.yaml
  type: apiKey
slug: passbolt-authentication
source_filename: passbolt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/passbolt-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerHttpAuthentication\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: Bearer token using a JWT\n  sources:\n  - openapi/passbolt-openapi.yaml\n- name: gpgCookieAuthentication\n  type: apiKey\n  in: cookie\n  parameter: passbolt_session\n  description: Session-based authentication. Note that a CSRF token needs to be provided through\n    a header named `X-CSRF-Token`.\n  sources:\n  - openapi/passbolt-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passbolt/refs/heads/main/authentication/passbolt-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Password Manager
- Security
- Secrets
- Identity
---
