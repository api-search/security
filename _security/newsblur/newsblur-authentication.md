---
api_key_in:
- cookie
api_specs:
- filename: newsblur-openapi.yml
  format: yaml
  label: NewsBlur API
  slug: newsblur-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Newsblur Authentication
name_suffix: Authentication
oauth_flows: []
overview: NewsBlur secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NewsBlur
provider_slug: newsblur
scheme_count: 2
schemes:
- description: Session cookie set by POST /api/login.
  in: cookie
  name: cookieAuth
  parameter: newsblur_sessionid
  sources:
  - openapi/newsblur-openapi.yml
  type: apiKey
- description: OAuth 2.0 access token passed as a Bearer token in the Authorization header. Client credentials are issued by NewsBlur (contact samuel@newsblur.com).
  name: oauth2Bearer
  scheme: bearer
  sources:
  - openapi/newsblur-openapi.yml
  type: http
slug: newsblur-authentication
source_filename: newsblur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/newsblur-openapi.yml\ndocs: https://www.newsblur.com/api\ndocs_notes: >-\n  The NewsBlur API reference documents two authentication paths: (1) a session cookie\n  (`newsblur_sessionid`) obtained via POST /api/login, and (2) OAuth 2.0 with a bearer\n  token in the Authorization header. OAuth client credentials are issued by NewsBlur\n  (contact samuel@newsblur.com). The same OAuth flow authorizes the hosted MCP server\n  at https://newsblur.com/mcp/ via a browser login-and-authorize step.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: newsblur_sessionid\n  description: Session cookie set by POST /api/login.\n  sources:\n  - openapi/newsblur-openapi.yml\n- name: oauth2Bearer\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token passed as a Bearer token in the Authorization header.\n    Client credentials are\
  \ issued by NewsBlur (contact samuel@newsblur.com).\n  sources:\n  - openapi/newsblur-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/authentication/newsblur-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- RSS
- News
- Feed Reader
- Aggregator
- Social
- Content
- Media
- Open Source
- MCP
---
