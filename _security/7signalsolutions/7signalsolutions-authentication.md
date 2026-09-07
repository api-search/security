---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 7signalsolutions-openapi.json
  format: json
  label: 7SIGNAL Platform API (Gateway v2)
  slug: 7signal-platform-api-gateway-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7signalsolutions/refs/heads/main/openapi/7signalsolutions-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 7Signalsolutions Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorization_code
overview: 7SIGNAL secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorization_code flow(s).
provider_name: 7SIGNAL
provider_slug: 7signalsolutions
scheme_count: 2
schemes:
- credential_terms:
    client_id: API Key
    client_secret: API Secret
    note: '7SIGNAL''s docs state plainly: "our API Key and Secret are just Client ID and Secret. We are using the same concept with simpler naming terms." Keys are created in the platform dashboard at https://start.7signal.com under Users -> API Keys, scoped to an Organization, Role and Sapphire Group.'
  failure_modes:
  - meaning: token missing, expired or invalid
    status: 401
  - meaning: token valid but lacks the required permission
    status: 403
  - error: invalid_grant
    meaning: grant_type missing or not client_credentials
  flows:
  - flow: clientCredentials
    scope_names:
    - read
    scopes: 1
    tokenUrl: https://api-v2.7signal.com/oauth2/token
  name: oauth2
  request_header: 'Authorization: Bearer <access_token>'
  sources:
  - https://github.com/7Signal/API-Examples/blob/develop/docs/01-authentication.md
  - https://github.com/7Signal/API-Examples/blob/develop/docs/04-api-keys.md
  - openapi/7signalsolutions-openapi.json
  surface: 7SIGNAL Platform API (Gateway v2)
  token:
    fixed: true
    format: JWT bearer
    lifetime_human: 24 hours
    lifetime_seconds: 86400
    refreshable: false
    response_fields:
    - access_token
    - scope
    - expires_in
    - token_type
    reuse_guidance: '"Tokens are only valid for 24 hours. This amount of time is fixed and cannot be changed. Once you acquire a token, reuse it for the duration of its validity." Do not request a new token per call.'
  type: oauth2
- bearer_methods_supported:
  - header
  discovery:
  - file: well-known/7signalsolutions-mcp-oauth-authorization-server.json
    path: /.well-known/oauth-authorization-server
    rfc: RFC 8414
    status: 200
  - file: well-known/7signalsolutions-mcp-oauth-protected-resource.json
    path: /.well-known/oauth-protected-resource
    rfc: RFC 9728
    status: 200
  flows:
  - authorizationUrl: https://mcp-v2.7signal.com/authorize
    flow: authorization_code
    pkce: S256
    registrationUrl: https://mcp-v2.7signal.com/register
    scopes: 9
    tokenUrl: https://mcp-v2.7signal.com/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: mcp_oauth
  sources:
  - https://mcp-v2.7signal.com/.well-known/oauth-authorization-server
  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource
  surface: 7SIGNAL MCP Server
  token_endpoint_auth_methods_supported:
  - client_secret_post
  type: oauth2
slug: 7signalsolutions-authentication
source_filename: 7signalsolutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://github.com/7Signal/API-Examples/blob/develop/docs/01-authentication.md\ndocs: https://github.com/7Signal/API-Examples/blob/develop/docs/01-authentication.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorization_code\n  surfaces: 2\n  note: >-\n    Two distinct OAuth 2.0 surfaces. The REST gateway (api-v2.7signal.com) uses the client-credentials\n    grant with a 7SIGNAL \"API Key\" and \"API Secret\" as client_id / client_secret. The remote MCP server\n    (mcp-v2.7signal.com) uses an authorization-code + PKCE flow with dynamic client registration,\n    advertised via RFC 8414 / RFC 9728 discovery documents.\nschemes:\n- name: oauth2\n  type: oauth2\n  surface: 7SIGNAL Platform API (Gateway v2)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-v2.7signal.com/oauth2/token\n    scopes: 1\n    scope_names:\n    - read\n  credential_terms:\n    client_id: API Key\n  \
  \  client_secret: API Secret\n    note: >-\n      7SIGNAL's docs state plainly: \"our API Key and Secret are just Client ID and Secret. We are using\n      the same concept with simpler naming terms.\" Keys are created in the platform dashboard at\n      https://start.7signal.com under Users -> API Keys, scoped to an Organization, Role and Sapphire Group.\n  token:\n    format: JWT bearer\n    lifetime_seconds: 86400\n    lifetime_human: 24 hours\n    fixed: true\n    refreshable: false\n    response_fields:\n    - access_token\n    - scope\n    - expires_in\n    - token_type\n    reuse_guidance: >-\n      \"Tokens are only valid for 24 hours. This amount of time is fixed and cannot be changed. Once you\n      acquire a token, reuse it for the duration of its validity.\" Do not request a new token per call.\n  request_header: 'Authorization: Bearer <access_token>'\n  failure_modes:\n  - status: 401\n    meaning: token missing, expired or invalid\n  - status: 403\n    meaning: token valid\
  \ but lacks the required permission\n  - error: invalid_grant\n    meaning: grant_type missing or not client_credentials\n  sources:\n  - https://github.com/7Signal/API-Examples/blob/develop/docs/01-authentication.md\n  - https://github.com/7Signal/API-Examples/blob/develop/docs/04-api-keys.md\n  - openapi/7signalsolutions-openapi.json\n- name: mcp_oauth\n  type: oauth2\n  surface: 7SIGNAL MCP Server\n  flows:\n  - flow: authorization_code\n    authorizationUrl: https://mcp-v2.7signal.com/authorize\n    tokenUrl: https://mcp-v2.7signal.com/token\n    registrationUrl: https://mcp-v2.7signal.com/register\n    pkce: S256\n    scopes: 9\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  bearer_methods_supported:\n  - header\n  discovery:\n  - path: /.well-known/oauth-authorization-server\n    rfc: RFC 8414\n    status: 200\n    file: well-known/7signalsolutions-mcp-oauth-authorization-server.json\n  - path:\
  \ /.well-known/oauth-protected-resource\n    rfc: RFC 9728\n    status: 200\n    file: well-known/7signalsolutions-mcp-oauth-protected-resource.json\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-authorization-server\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\napi_key_management:\n  create_path: https://start.7signal.com -> Users -> API Keys -> Add\n  scoped_by:\n  - Organization\n  - Role\n  - Sapphire Group\n  api_operations:\n  - apikeys-get-e5f6\n  - apikeys-post-g7h8\n  - apikeys-with-id-get-i9j0\n  - apikeys-with-id-delete-k1l2\n  source: https://github.com/7Signal/API-Examples/blob/develop/README.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7signalsolutions/refs/heads/main/authentication/7signalsolutions-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Wireless Network Monitoring
- Wi-Fi Experience Monitoring
- Digital Experience Monitoring
- Network Performance Monitoring
- Network Observability
- AIOps
- IT Operations
- Endpoint Monitoring
- Time Series
- MCP
- agent-native
- Company
---
