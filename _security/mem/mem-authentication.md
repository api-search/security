---
api_key_in:
- header
- query
api_specs:
- filename: mem-openapi-original.json
  format: json
  label: Mem Public Client API
  slug: mem-public-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem/refs/heads/main/openapi/mem-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mem Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Mem secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Mem
provider_slug: mem
scheme_count: 3
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mem-openapi-original.json
  type: http
- in: query
  name: CoreApi__AssetAccessToken
  parameter: token
  sources:
  - openapi/mem-openapi-original.json
  type: apiKey
- in: header
  name: CoreApi__Authorization
  parameter: Authorization
  sources:
  - openapi/mem-openapi-original.json
  type: apiKey
slug: mem-authentication
source_filename: mem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mem-openapi-original.json\ndocs: https://docs.mem.ai/api-reference/overview/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  primary: >-\n    REST API requests authenticate with a personal bearer token\n    (Authorization: Bearer $MEM_API_KEY) created in Mem settings. OAuth 2.0 is\n    used for the hosted MCP server and third-party app connectors, advertised\n    via RFC 8414 / OIDC discovery on api.mem.ai (scopes content.read,\n    content.write, profile.read, profile.write). See scopes/mem-scopes.yml.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mem-openapi-original.json\n- name: CoreApi__AssetAccessToken\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/mem-openapi-original.json\n- name: CoreApi__Authorization\n  type: apiKey\n\
  \  in: header\n  parameter: Authorization\n  sources:\n  - openapi/mem-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mem/refs/heads/main/authentication/mem-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Notes
- Knowledge Management
- Productivity
- Artificial Intelligence
- Note Taking
- Search
- MCP
- Agents
- Meetings
---
