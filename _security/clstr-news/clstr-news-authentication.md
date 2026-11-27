---
anonymous_access: true
api_key_in: []
api_specs:
- filename: clstr-news-openapi-generated.yml
  format: yaml
  label: CLSTR API
  slug: clstr-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clstr-news/openapi/_ae-authored/clstr-news-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CLSTR Authentication
name_suffix: Authentication
oauth_flows: []
overview: CLSTR declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: CLSTR
provider_slug: clstr-news
scheme_count: 4
schemes:
- format: 'Authorization: Bearer clstr_YOUR_KEY'
  header: Authorization
  in: header
  key_prefix: clstr_
  name: bearerAuth
  scheme: bearer
  surfaces:
  - rest
  - mcp
  type: http
- header: X-Api-Key
  in: header
  name: apiKeyHeader
  note: Docs state the key may be sent "as an `X-Api-Key` header" as an alternative to Bearer.
  surfaces:
  - rest
  type: apiKey
- name: mcpOAuth
  note: MCP assistant connectors (Claude, ChatGPT) run "an OAuth sign-in against your account". Flows, endpoints and scopes are not documented; not probed (auth endpoints are out of bounds).
  surfaces:
  - mcp
  type: oauth2
- name: anonymous
  note: Keyless MCP taster for get_top_situations and get_situation_timeline, 3 calls per day per network.
  surfaces:
  - mcp
  type: none
slug: clstr-news-authentication
source_filename: clstr-news-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clstr.news/developers.md\ndocs: https://clstr.news/developers#authentication\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer clstr_YOUR_KEY'\n  key_prefix: clstr_\n  surfaces: [rest, mcp]\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  header: X-Api-Key\n  surfaces: [rest]\n  note: Docs state the key may be sent \"as an `X-Api-Key` header\" as an alternative to Bearer.\n- name: mcpOAuth\n  type: oauth2\n  surfaces: [mcp]\n  note: 'MCP assistant connectors (Claude, ChatGPT) run \"an OAuth sign-in against your account\". Flows, endpoints and scopes are not documented; not probed (auth endpoints are out of bounds).'\n- name: anonymous\n  type: none\n  surfaces: [mcp]\n  note: Keyless MCP taster for get_top_situations and get_situation_timeline, 3 calls per day per network.\nkey_management:\n  issuance: Create a free API key in\
  \ Settings (https://clstr.news/settings). Sign in first, no card needed.\n  max_active_keys_per_account: 5\n  guidance: Keys are secrets; call the API from your own server, not front-end JavaScript.\n"
source_yaml_url: https://artifacts.apis.io/clstr-news/authentication/clstr-news-authentication.yml
summary_line: 4 schemes
tags:
- Company
- News
- News API
- MCP
- AI Agents
- News Clustering
- Media Monitoring
- Summarization
---
