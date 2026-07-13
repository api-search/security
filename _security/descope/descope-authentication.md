---
api_key_in: []
api_specs:
- filename: descope-openapi.yml
  format: yaml
  label: Descope Authentication API
  slug: descope-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope Management API
  slug: descope-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope OAuth Applications API
  slug: descope-oauth-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope SCIM 2.0 API
  slug: descope-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope JWKS and Discovery API
  slug: descope-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Descope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Descope secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Descope
provider_slug: descope
scheme_count: 1
schemes:
- bearerFormat: Project ID
  description: Project ID as bearer token.
  name: Descope Project ID
  scheme: bearer
  sources:
  - openapi/descope-openapi.yml
  type: http
slug: descope-authentication
source_filename: descope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/descope-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Descope Project ID\n  type: http\n  scheme: bearer\n  bearerFormat: Project ID\n  description: Project ID as bearer token.\n  sources:\n  - openapi/descope-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/authentication/descope-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity
- CIAM
- Passwordless
- Passkeys
- MFA
- SSO
- OAuth
- OIDC
- SAML
- SCIM
- Authorization
- FGA
- Agentic Identity
- MCP
---
