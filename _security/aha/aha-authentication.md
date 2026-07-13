---
api_key_in:
- cookie
api_specs:
- filename: openapi.json
  format: json
  label: Aha.io REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://www.aha.io/openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aha Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Aha.io secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Aha.io
provider_slug: aha
scheme_count: 3
schemes:
- description: OAuth2 authentication with bearer tokens
  flows:
  - authorizationUrl: https://{account-domain}.aha.io/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{account-domain}.aha.io/oauth/token
  name: OAuth2
  sources:
  - openapi/aha-openapi.json
  type: oauth2
- description: API key authentication using Bearer token in Authorization header. Generate API keys at https://secure.aha.io/settings/api_keys
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/aha-openapi.json
  type: http
- description: Cookie-based authentication for web browser integration
  in: cookie
  name: CookieAuth
  parameter: session
  sources:
  - openapi/aha-openapi.json
  type: apiKey
slug: aha-authentication
source_filename: aha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aha-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{account-domain}.aha.io/oauth/authorize\n    tokenUrl: https://{account-domain}.aha.io/oauth/token\n    scopes: 0\n  description: OAuth2 authentication with bearer tokens\n  sources:\n  - openapi/aha-openapi.json\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API key authentication using Bearer token in Authorization header. Generate API\n    keys at https://secure.aha.io/settings/api_keys\n  sources:\n  - openapi/aha-openapi.json\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Cookie-based authentication for web browser integration\n  sources:\n  - openapi/aha-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aha/refs/heads/main/authentication/aha-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Product Management
- Roadmapping
- Idea Management
- Product Development
- Requirements
- Agile
---
