---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Polymer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polymer declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Polymer
provider_slug: polymer
scheme_count: 3
schemes:
- description: Workspace API key sent in the X-API-KEY request header. This is the recommended way to authenticate server-to-server calls.
  id: api_key_header
  in: header
  name: X-API-KEY
  type: apiKey
- description: Workspace API key supplied as the api_key query-string parameter, equivalent to the X-API-KEY header.
  id: api_key_query
  in: query
  name: api_key
  type: apiKey
- description: 'Short-lived embed token minted via GET /v1/auth/token. Passed as the ptoken query parameter on the embed URL (https://v3.polymersearch.com/b/{board_id}?ptoken={token}) to render a permission-scoped board to an end user who has no Polymer account. Permission levels: board_read_only, board_edit, workspace_read_only, workspace_edit, block_level_read_only.'
  id: embed_token
  in: query
  name: ptoken
  type: apiKey
slug: polymer-authentication
source_filename: polymer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://apidocs.polymersearch.com/\napi: Polymer Embedded Analytics API\nname: Polymer Authentication Profile\nsummary: >-\n  The Polymer API authenticates every request with a workspace API key. The key\n  may be sent as an X-API-KEY request header or as an api_key query-string\n  parameter. Short-lived embed tokens are minted from the API to grant\n  permission-scoped, account-less access to end users of embedded dashboards.\nschemes:\n- id: api_key_header\n  type: apiKey\n  in: header\n  name: X-API-KEY\n  description: >-\n    Workspace API key sent in the X-API-KEY request header. This is the\n    recommended way to authenticate server-to-server calls.\n- id: api_key_query\n  type: apiKey\n  in: query\n  name: api_key\n  description: >-\n    Workspace API key supplied as the api_key query-string parameter,\n    equivalent to the X-API-KEY header.\n- id: embed_token\n  type: apiKey\n  in: query\n  name: ptoken\n  description:\
  \ >-\n    Short-lived embed token minted via GET /v1/auth/token. Passed as the ptoken\n    query parameter on the embed URL (https://v3.polymersearch.com/b/{board_id}?ptoken={token})\n    to render a permission-scoped board to an end user who has no Polymer\n    account. Permission levels: board_read_only, board_edit, workspace_read_only,\n    workspace_edit, block_level_read_only.\nheaders:\n  workspace_scope: >-\n    An optional workspace-id header targets a workspace other than the API key's\n    default workspace.\nnotes:\n- No OAuth 2.0 / OpenID Connect flows are documented; access is API-key based.\n- No machine-readable OpenAPI security scheme is published; this profile was\n  derived by reading the developer documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polymer/refs/heads/main/authentication/polymer-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Analytics
- Business Intelligence
- Data Visualization
- Embedded Analytics
- Dashboards
- Data
- Artificial Intelligence
---
