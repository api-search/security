---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Incorta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Incorta secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Incorta
provider_slug: incorta
scheme_count: 2
schemes:
- description: 'PAT generated in the Incorta Profile Manager. Sent as ''Authorization: Bearer {PAT}''.'
  name: personalAccessToken
  scheme: bearer
  sources:
  - docs
  type: http
- bearerFormat: JWT
  description: 'OAuth 2.0 JWT issued by a user-configured OAuth 2.0 authorization server; sent as ''Authorization: Bearer {JWT}''. Scopes/claims are defined by the external authorization server, not by Incorta.'
  name: oauth2Jwt
  scheme: bearer
  sources:
  - docs
  type: http
slug: incorta-authentication
source_filename: incorta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.incorta.com/latest/references-public-api-v2/\ndocs: https://docs.incorta.com/latest/references-public-api-v2/\n# Incorta Public API v2 authenticates with a bearer access token that is either a\n# Personal Access Token (PAT) or an OAuth 2.0 JWT issued by a user-configured\n# OAuth 2.0 authorization server. A Super User / SuperRole first enables public\n# API access for the user or group. (v1 used a generated API key instead.)\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  token_kinds: [personal-access-token, oauth2-jwt]\n  authorization_model: role-based (SuperRole, Schema Manager, entity access rights)\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: >-\n    PAT generated in the Incorta Profile Manager. Sent as\n    'Authorization: Bearer {PAT}'.\n  sources: [docs]\n- name: oauth2Jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n   \
  \ OAuth 2.0 JWT issued by a user-configured OAuth 2.0 authorization server;\n    sent as 'Authorization: Bearer {JWT}'. Scopes/claims are defined by the\n    external authorization server, not by Incorta.\n  sources: [docs]\nnotes:\n- Public API access must be enabled per user/group by a Super User or SuperRole.\n- v1 (releases 5.0+) authenticated with a generated API key; v2 (6.0+) uses PAT or JWT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incorta/refs/heads/main/authentication/incorta-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Enterprise
- Analytics
- Business Intelligence
- Data Platform
- Data Analytics
- Data Integration
- Dashboards
---
