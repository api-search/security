---
api_key_in: []
api_specs:
- filename: v1
  format: yaml
  label: Beyond Identity Secure Access API
  slug: beyond-identity-secure-access-api
  spec_type: OpenAPI
  url: https://developer.beyondidentity.com/api/v1
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Beyond Identity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beyond Identity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Beyond Identity
provider_slug: beyond-identity
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: See the [Authentication](#section/Authentication) section for details.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/beyond-identity-secure-access-api-openapi.yml
  - openapi/beyond-identity-secure-workforce-api-openapi.yml
  type: http
slug: beyond-identity-authentication
source_filename: beyond-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beyond-identity-secure-access-api-openapi.yml, openapi/beyond-identity-secure-workforce-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: See the [Authentication](#section/Authentication) section for details.\n  sources:\n  - openapi/beyond-identity-secure-access-api-openapi.yml\n  - openapi/beyond-identity-secure-workforce-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/authentication/beyond-identity-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Passwordless
- Zero Trust
- Identity
- Passkeys
- MFA
- Device Security
- OAuth 2.0
- OIDC
- SCIM
---
