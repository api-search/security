---
api_key_in:
- header
api_specs:
- filename: slashid-openapi-latest.yaml
  format: yaml
  label: SlashID API
  slug: slashid-api
  spec_type: OpenAPI
  url: https://cdn.slashid.com/slashid-openapi-latest.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Slashid Authentication
name_suffix: Authentication
oauth_flows: []
overview: SlashID secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SlashID
provider_slug: slashid
scheme_count: 3
schemes:
- description: Authorizes the request with the organization's API Key.
  in: header
  name: ApiKeyAuth
  parameter: SlashID-API-Key
  sources:
  - openapi/slashid-api-openapi.yml
  type: apiKey
- description: Authorizes the request with a client ID/client secret pair
  name: OAuth2ClientIdSecret
  scheme: basic
  sources:
  - openapi/slashid-api-openapi.yml
  type: http
- bearerFormat: opaque
  description: Authorizes the request with an Access Token for the current user.
  name: OAuth2AccessTokenBearer
  scheme: bearer
  sources:
  - openapi/slashid-api-openapi.yml
  type: http
slug: slashid-authentication
source_filename: slashid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/slashid-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: SlashID-API-Key\n  description: Authorizes the request with the organization's API Key.\n  sources:\n  - openapi/slashid-api-openapi.yml\n- name: OAuth2ClientIdSecret\n  type: http\n  scheme: basic\n  description: Authorizes the request with a client ID/client secret pair\n  sources:\n  - openapi/slashid-api-openapi.yml\n- name: OAuth2AccessTokenBearer\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: Authorizes the request with an Access Token for the current user.\n  sources:\n  - openapi/slashid-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slashid/refs/heads/main/authentication/slashid-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Identity
- Authentication
- Passwordless
- MFA
- Passkeys
- User Management
- CIAM
- OAuth2
- OIDC
- SSO
- RBAC
- Security
---
