---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Promethium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Promethium declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Promethium
provider_slug: promethium
scheme_count: 5
schemes:
- description: Interactive browser-based authentication. Redirects to the tenant's configured SSO provider and returns id_token, access_token, and refresh_token.
  flow: browser-redirect (SSO / OIDC provider)
  id: oauth2-sso
  login: GET /auth/login/{tenant}
  type: oauth2
- body: '{ "email": "<email>", "password": "<password>" }'
  content_type: application/json
  description: Direct credential exchange for local service accounts.
  flow: password (resource owner credentials)
  id: oauth2-service-account
  login: POST /auth/login/{tenant}
  returns:
  - id_token
  - access_token
  - refresh_token
  type: oauth2
- description: The id_token obtained from /auth/login must be sent in the "idtoken" header on all subsequent API calls (custom header, not RFC 6750 Bearer).
  id: idtoken-header
  in: header
  name: idtoken
  type: apiKey
- applies_to: Trino Stream query endpoint
  header: 'Authorization: Basic <base64>'
  id: trino-basic
  scheme: basic
  type: http
- applies_to: Trino Stream query endpoint
  header: 'Authorization: Bearer <token>'
  id: trino-bearer
  scheme: bearer
  type: http
slug: promethium-authentication
source_filename: promethium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.promethium.ai/docs/api-reference/api-auth + api-trino-stream-auth\nname: Promethium API Authentication\nbase_url: https://api.prod.promethium.ai\ndocs: https://docs.promethium.ai/docs/api-reference/api-auth\nsummary: >-\n  Promethium uses tenant-scoped OAuth2 token authentication. Interactive SSO users\n  authenticate via a browser redirect flow; local service accounts exchange\n  email/password credentials for tokens. The returned id_token is passed on every\n  subsequent request in a custom \"idtoken\" header (not a standard Bearer header).\n  The Trino Stream query surface additionally accepts HTTP Basic and OAuth2 Bearer.\nschemes:\n- id: oauth2-sso\n  type: oauth2\n  flow: browser-redirect (SSO / OIDC provider)\n  login: GET /auth/login/{tenant}\n  description: >-\n    Interactive browser-based authentication. Redirects to the tenant's configured\n    SSO provider and returns id_token, access_token, and refresh_token.\n\
  - id: oauth2-service-account\n  type: oauth2\n  flow: password (resource owner credentials)\n  login: POST /auth/login/{tenant}\n  content_type: application/json\n  body: '{ \"email\": \"<email>\", \"password\": \"<password>\" }'\n  returns: [id_token, access_token, refresh_token]\n  description: Direct credential exchange for local service accounts.\n- id: idtoken-header\n  type: apiKey\n  in: header\n  name: idtoken\n  description: >-\n    The id_token obtained from /auth/login must be sent in the \"idtoken\" header on\n    all subsequent API calls (custom header, not RFC 6750 Bearer).\n- id: trino-basic\n  type: http\n  scheme: basic\n  applies_to: Trino Stream query endpoint\n  header: 'Authorization: Basic <base64>'\n- id: trino-bearer\n  type: http\n  scheme: bearer\n  applies_to: Trino Stream query endpoint\n  header: 'Authorization: Bearer <token>'\ntoken_lifecycle:\n  refresh: 'POST /auth/refresh/{tenant} (body: refresh_token)'\n  logout: 'GET /auth/logout/{tenant}'\nnotes:\n\
  - Authentication and all hosts are tenant-scoped ({tenant}) and environment-scoped ({env}, e.g. prod).\n- No public OAuth scopes are documented; authorization is enforced via roles/domains (see docs/authorization).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/promethium/refs/heads/main/authentication/promethium-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Data Fabric
- Agentic Analytics
- Semantic Layer
- Enterprise Data
- Model Context Protocol
- Federated Query
- Data Governance
---
