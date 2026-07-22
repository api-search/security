---
api_key_in:
- header
auth_types:
- apiKey
description: The Verkada Command API uses a two-tier API key + short-lived token model (adopted November 2024). Organization admins mint a scoped, long-lived API Key in Command (Organization Settings > Verkada API), choosing product/endpoint permission sets and a Read-only or Read/Write scope. The API Key is never sent to endpoints directly; instead it is exchanged for a short-lived API Token that is used to authenticate individual endpoint calls.
kind: authentication
layout: security
method: searched
name: Verkada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verkada secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verkada
provider_slug: verkada
scheme_count: 3
schemes:
- in: header
  name: apiKey
  notes: Scoped, org-admin-created. Permissions are fixed at creation time and cannot be edited. Max lifetime 20 years; Verkada recommends <= 1 year and annual rotation. Legacy (pre-Nov-2024) API keys remain valid until their existing expiration and can still call endpoints directly.
  parameter_name: x-api-key
  role: top-level key (used only against the token endpoint and streaming-token endpoints)
  sources:
  - https://apidocs.verkada.com/reference/quick-start-guide
  type: apiKey
- in: header
  lifetime_seconds: 1800
  mint_operation: postloginapikeyviewv2
  name: apiToken
  notes: POST the top-level API Key as the x-api-key header to /token to receive {"token":"v2_api_token"}. Valid for 30 minutes, cannot be refreshed - mint a new token when expired. Tokens inherit the permission scope of the API Key that minted them. Expired tokens return HTTP 401 with body {"id":"0e2d","message":"Token expired","data":null}.
  parameter_name: x-verkada-auth
  refreshable: false
  role: short-lived endpoint token
  sources:
  - https://apidocs.verkada.com/reference/postloginapikeyviewv2
  token_endpoint: https://api.verkada.com/token
  type: apiKey
- bearerFormat: JWT
  in: query
  lifetime_seconds: 1800
  mint_operation: getfootagetokenviewv1
  name: streamingJwt
  notes: Live/historical HLS footage streaming uses a separate JWT obtained from the Get Streaming Token endpoint (which itself requires the top-level API Key). The JWT is passed as a query parameter to the streaming endpoint and is valid for 30 minutes.
  parameter_name: jwt
  role: footage streaming token
  scheme: bearer
  sources:
  - https://apidocs.verkada.com/reference/getfootagetokenviewv1
  type: http
slug: verkada-authentication
source_filename: verkada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://apidocs.verkada.com/reference/quick-start-guide\ndocs: https://apidocs.verkada.com/reference/security-overview\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  model: two-tier-key-token\n  oauth2_flows: []\ndescription: >-\n  The Verkada Command API uses a two-tier API key + short-lived token model\n  (adopted November 2024). Organization admins mint a scoped, long-lived API Key\n  in Command (Organization Settings > Verkada API), choosing product/endpoint\n  permission sets and a Read-only or Read/Write scope. The API Key is never sent\n  to endpoints directly; instead it is exchanged for a short-lived API Token that\n  is used to authenticate individual endpoint calls.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  role: top-level key (used only against the token endpoint and streaming-token endpoints)\n  notes: >-\n    Scoped, org-admin-created. Permissions are fixed\
  \ at creation time and cannot\n    be edited. Max lifetime 20 years; Verkada recommends <= 1 year and annual\n    rotation. Legacy (pre-Nov-2024) API keys remain valid until their existing\n    expiration and can still call endpoints directly.\n  sources: [https://apidocs.verkada.com/reference/quick-start-guide]\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter_name: x-verkada-auth\n  role: short-lived endpoint token\n  mint_operation: postloginapikeyviewv2\n  token_endpoint: https://api.verkada.com/token\n  lifetime_seconds: 1800\n  refreshable: false\n  notes: >-\n    POST the top-level API Key as the x-api-key header to /token to receive\n    {\"token\":\"v2_api_token\"}. Valid for 30 minutes, cannot be refreshed - mint a\n    new token when expired. Tokens inherit the permission scope of the API Key\n    that minted them. Expired tokens return HTTP 401 with body\n    {\"id\":\"0e2d\",\"message\":\"Token expired\",\"data\":null}.\n  sources: [https://apidocs.verkada.com/reference/postloginapikeyviewv2]\n\
  - name: streamingJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  role: footage streaming token\n  mint_operation: getfootagetokenviewv1\n  in: query\n  parameter_name: jwt\n  lifetime_seconds: 1800\n  notes: >-\n    Live/historical HLS footage streaming uses a separate JWT obtained from the\n    Get Streaming Token endpoint (which itself requires the top-level API Key).\n    The JWT is passed as a query parameter to the streaming endpoint and is valid\n    for 30 minutes.\n  sources: [https://apidocs.verkada.com/reference/getfootagetokenviewv1]\nnotes:\n- The Camera Audio API requires a separate \"Camera Audio\" API key distinct from Read-only and Read/Write keys.\n- All requests must be made over HTTPS (TLS 1.2 or 1.3, AES-128).\n- Credentials are region-bound and only work against the region where the org was created.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verkada/refs/heads/main/authentication/verkada-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Security
- Physical Security
- Video Surveillance
- Access Control
- Cameras
- Sensors
- Alarms
- IoT
- Cloud
- Webhooks
- Building Management
---
