---
api_key_in: []
api_specs:
- filename: propelauth-user-api-openapi.yml
  format: yaml
  label: PropelAuth User API
  slug: propelauth-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-user-api-openapi.yml
- filename: propelauth-org-api-openapi.yml
  format: yaml
  label: PropelAuth Organization API
  slug: propelauth-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-org-api-openapi.yml
- filename: propelauth-api-keys-api-openapi.yml
  format: yaml
  label: PropelAuth End-User API Keys API
  slug: propelauth-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-api-keys-api-openapi.yml
- filename: propelauth-oauth2-api-openapi.yml
  format: yaml
  label: PropelAuth OAuth2 API
  slug: propelauth-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-oauth2-api-openapi.yml
- filename: propelauth-mcp-api-openapi.yml
  format: yaml
  label: PropelAuth MCP Authentication API
  slug: propelauth-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Propelauth Authentication
name_suffix: Authentication
oauth_flows: []
overview: PropelAuth secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PropelAuth
provider_slug: propelauth
scheme_count: 1
schemes:
- name: BackendApiKey
  scheme: bearer
  sources:
  - openapi/propelauth-api-keys-api-openapi.yml
  - openapi/propelauth-oauth2-api-openapi.yml
  - openapi/propelauth-org-api-openapi.yml
  - openapi/propelauth-user-api-openapi.yml
  type: http
slug: propelauth-authentication
source_filename: propelauth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/propelauth-api-keys-api-openapi.yml, openapi/propelauth-oauth2-api-openapi.yml,\n  openapi/propelauth-org-api-openapi.yml, openapi/propelauth-user-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BackendApiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/propelauth-api-keys-api-openapi.yml\n  - openapi/propelauth-oauth2-api-openapi.yml\n  - openapi/propelauth-org-api-openapi.yml\n  - openapi/propelauth-user-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/authentication/propelauth-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity
- B2B
- Multi-Tenancy
- Authorization
- RBAC
- SSO
- SCIM
- MCP
- API Keys
---
