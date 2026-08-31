---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hello Therma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hello Therma declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hello Therma
provider_slug: hello-therma
scheme_count: 1
schemes:
- applies_to:
  - https://mcp.glaciergrid.com/mcp
  authorization_endpoint: https://mcp.glaciergrid.com/authorize
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: glaciergrid_mcp_oauth
  issuer: https://mcp.glaciergrid.com/
  pkce:
    required_methods:
    - S256
  registration_endpoint: https://mcp.glaciergrid.com/register
  response_types_supported:
  - code
  revocation_endpoint: https://mcp.glaciergrid.com/revoke
  revocation_endpoint_auth_methods_supported:
  - client_secret_post
  scopes_supported:
  - internal
  - customer
  service_documentation: https://glaciergrid.com/
  token_endpoint: https://mcp.glaciergrid.com/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
slug: hello-therma-authentication
source_filename: hello-therma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://mcp.glaciergrid.com/.well-known/oauth-authorization-server\ndocs: https://www.glaciergrid.com/connector\nsummary: >-\n  GlacierGrid's only public machine-callable surface — the remote MCP server at\n  https://mcp.glaciergrid.com/mcp — is protected by OAuth 2.1 authorization-code flow with\n  PKCE, and it publishes both RFC 8414 authorization-server metadata and RFC 9728\n  protected-resource metadata. There is no API-key surface, no basic auth, and no\n  unauthenticated read path. There is no OpenAPI document to derive securitySchemes from;\n  everything below was read from the server's own live metadata.\n\nschemes:\n- id: glaciergrid_mcp_oauth\n  type: oauth2\n  flow: authorization_code\n  pkce:\n    required_methods:\n    - S256\n  issuer: https://mcp.glaciergrid.com/\n  authorization_endpoint: https://mcp.glaciergrid.com/authorize\n  token_endpoint: https://mcp.glaciergrid.com/token\n  revocation_endpoint: https://mcp.glaciergrid.com/revoke\n\
  \  registration_endpoint: https://mcp.glaciergrid.com/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - none\n  revocation_endpoint_auth_methods_supported:\n  - client_secret_post\n  scopes_supported:\n  - internal\n  - customer\n  applies_to:\n  - https://mcp.glaciergrid.com/mcp\n  service_documentation: https://glaciergrid.com/\n\ndynamic_client_registration:\n  supported: true\n  endpoint: https://mcp.glaciergrid.com/register\n  spec: RFC 7591\n  evidence: >-\n    POST https://mcp.glaciergrid.com/register with an empty JSON body returned 400 (the\n    endpoint exists and validates its input) and the endpoint is advertised in the\n    authorization-server metadata as registration_endpoint.\n\nchallenge:\n  status: 401\n  header: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.glaciergrid.com/.well-known/oauth-protected-resource/mcp\"'\n \
  \ body: '{\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Unauthorized: Bearer token required\"},\"id\":null}'\n  note: >-\n    The 401 carries a resource_metadata pointer, so an MCP client can discover the\n    authorization server with no out-of-band configuration. This is the RFC 9728 pattern.\n\nend_user_flow:\n  described_at: https://www.glaciergrid.com/connector\n  requires:\n  - An active GlacierGrid account\n  - GlacierGrid login credentials\n  identity_provider_note: >-\n    GlacierGrid's published subprocessor list names Google (Firebase) for \"Identity and\n    sign-in\" and AWS ElastiCache (Valkey) for \"Authorization state only; no facility data\".\n  identity_provider_source: https://www.glaciergrid.com/subprocessors\n\nnot_present:\n- api_key\n- http_basic\n- http_bearer_static\n- mutual_tls\n- openid_connect_discovery\nnotes:\n- >-\n  /.well-known/openid-configuration returns 404 on mcp.glaciergrid.com — the server is an\n  OAuth 2.0 authorization server (RFC\
  \ 8414), not an OpenID Connect provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-therma/refs/heads/main/authentication/hello-therma-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Internet of Things
- Energy
- Sustainability
- Cold Chain
- Temperature Monitoring
- Refrigeration
- HVAC
- Building Automation
- Food Safety
- Facilities Management
- Restaurant
- Retail
- MCP
- Agents
---
