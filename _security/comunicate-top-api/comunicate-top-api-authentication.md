---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Comunicate.top API
  slug: comunicatetop-api
  spec_type: OpenAPI
  url: https://comunicate.top/openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Comunicate Top Api Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Comunicate.top API secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Comunicate.top API
provider_slug: comunicate-top-api
scheme_count: 2
schemes:
- description: API key from Integrations (bk_live_…)
  name: apiKey
  scheme: bearer
  sources:
  - openapi/comunicate-top-api-openapi-original.json
  type: http
- description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.top/api/v1/oauth/register. The access token is an API key and is accepted everywhere an API key is.
  flows:
  - authorizationUrl: https://app.comunicate.top/api/v1/oauth/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://app.comunicate.top/api/v1/oauth/token
  name: oauth2
  sources:
  - openapi/comunicate-top-api-openapi-original.json
  type: oauth2
slug: comunicate-top-api-authentication
source_filename: comunicate-top-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: derived\nsource: openapi/comunicate-top-api-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from Integrations (bk_live_…)\n  sources:\n  - openapi/comunicate-top-api-openapi-original.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.comunicate.top/api/v1/oauth/authorize\n    tokenUrl: https://app.comunicate.top/api/v1/oauth/token\n    scopes: 10\n  description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.top/api/v1/oauth/register.\n    The access token is an API key and is accepted everywhere an API key is.\n  sources:\n  - openapi/comunicate-top-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/authentication/comunicate-top-api-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Press Releases
- Advertorials
- PR
- Publishing
- Media
- SEO
- Link Building
- Content Marketing
- Romania
- MCP
- Open Data
- Webhooks
- OAuth
---
