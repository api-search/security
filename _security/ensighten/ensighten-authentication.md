---
api_key_in:
- header
api_specs:
- filename: ensighten-manage-api-openapi.yml
  format: yaml
  label: Ensighten Manage API
  slug: manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ensighten/refs/heads/main/openapi/ensighten-manage-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ensighten Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Ensighten secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Ensighten
provider_slug: ensighten
scheme_count: 3
schemes:
- description: API Key created in the Admin > API Keys page of Manage. Keys are prefixed 'ens_'. Not accepted on /auth/token.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/ensighten-manage-api-openapi.yml
  type: apiKey
- description: Access token obtained from POST /auth/token (OAuth 2.0 Resource Owner Password Credentials flow).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ensighten-manage-api-openapi.yml
  type: http
- description: Resource Owner Password Credentials flow. No OAuth scopes are documented; authorization is governed by Manage Roles assigned to the user or API Key.
  flows:
  - flow: password
    scopes: 0
    tokenUrl: https://manage-api.ensighten.com/auth/token
  name: OAuth2Password
  sources:
  - openapi/ensighten-manage-api-openapi.yml
  type: oauth2
slug: ensighten-authentication
source_filename: ensighten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/ensighten-manage-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API Key created in the Admin > API Keys page of Manage. Keys are prefixed 'ens_'.\n    Not accepted on /auth/token.\n  sources:\n  - openapi/ensighten-manage-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Access token obtained from POST /auth/token (OAuth 2.0 Resource Owner Password\n    Credentials flow).\n  sources:\n  - openapi/ensighten-manage-api-openapi.yml\n- name: OAuth2Password\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://manage-api.ensighten.com/auth/token\n    scopes: 0\n  description: Resource Owner Password Credentials flow. No OAuth scopes are documented; authorization\n    is governed by Manage Roles assigned\
  \ to the user or API Key.\n  sources:\n  - openapi/ensighten-manage-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ensighten/refs/heads/main/authentication/ensighten-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Cybersecurity
- Tag Management
- Data Governance
- Client-Side Security
- Consent Management
- Privacy Compliance
- Marketing Technology
---
