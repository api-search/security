---
api_key_in: []
api_specs:
- filename: velaris-openapi.yml
  format: yaml
  label: Velaris Public API
  slug: velaris-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Velaris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Velaris secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Velaris
provider_slug: velaris
scheme_count: 2
schemes:
- description: 'User-scoped access token. Header: Authorization: Bearer {access_token}. Create under Profile > Security > Access token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/velaris-openapi.yml
  type: http
- description: Legacy. Base64(username:password). Not available for SSO/MFA tenants.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/velaris-openapi.yml
  type: http
slug: velaris-authentication
source_filename: velaris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.velaris.io/ (auth section) + openapi/velaris-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'User-scoped access token. Header: Authorization: Bearer {access_token}. Create under Profile > Security\n    > Access token.'\n  sources:\n  - openapi/velaris-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Legacy. Base64(username:password). Not available for SSO/MFA tenants.\n  sources:\n  - openapi/velaris-openapi.yml\ndocs: https://developers.velaris.io/\ndetail: 'Two options: (1) Token-based - any user creates a user-scoped API token in-app under Profile > Security\n  > Access token, sent as Authorization: Bearer {access_token}; works for SSO and non-SSO tenants. (2) Basic authentication\n  (legacy) - Base64(username:password) of an administrator-privileged user, sent as Authorization: Basic {token};\n  not available\
  \ for SSO-enabled tenants.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/authentication/velaris-authentication.yml
summary_line: http · 2 schemes
tags:
- Customer Success
- AI
- SaaS
- Customer Data
- CRM
- Analytics
- Automation
- Company
---
