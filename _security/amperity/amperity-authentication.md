---
api_key_in: []
api_specs:
- filename: amperity-audit-events-api-openapi.yml
  format: yaml
  label: Amperity Audit Events API
  slug: amperity-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-audit-events-api-openapi.yml
- filename: amperity-campaigns-api-openapi.yml
  format: yaml
  label: Amperity Campaigns API
  slug: amperity-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-campaigns-api-openapi.yml
- filename: amperity-ingest-api-openapi.yml
  format: yaml
  label: Amperity Ingest API
  slug: amperity-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-ingest-api-openapi.yml
- filename: amperity-segments-api-openapi.yml
  format: yaml
  label: Amperity Segments API
  slug: amperity-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-segments-api-openapi.yml
- filename: amperity-workflow-api-openapi.yml
  format: yaml
  label: Amperity Workflow API
  slug: amperity-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-workflow-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Amperity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Amperity secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Amperity
provider_slug: amperity
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    grant_type: client_credentials
    request_content_type: application/x-www-form-urlencoded
    request_params:
    - client_id
    - client_secret
    scopes: {}
    tokenUrl: https://{tenant}.amperity.com/api/v0/oauth2/token
    token_response:
      access_token: string
      expires_in: 3600
      token_type: Bearer
  name: OAuth2ClientCredentials
  sources:
  - https://docs.amperity.com/api/authentication.html
  type: oauth2
- applied_via: 'Authorization: Bearer ${access-token}'
  bearerFormat: JWT
  name: BearerJWT
  scheme: bearer
  sources:
  - https://docs.amperity.com/api/authentication.html
  type: http
slug: amperity-authentication
source_filename: amperity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.amperity.com/api/authentication.html\ndocs: https://docs.amperity.com/api/authentication.html\nsummary:\n  types: [oauth2, http]\n  http_scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials, authorizationCode]\n  surfaces: 2\n  surfaces_note: >-\n    Amperity runs TWO separate OAuth2 deployments with different flows, different token endpoints and\n    different identity models. The REST APIs use client-credentials against a tenant token endpoint and\n    authenticate a SYNTHETIC IDENTITY (an API key). The hosted MCP server uses authorization-code with\n    PKCE against mcp.amperity.com and authenticates a REAL HUMAN USER, scoping every request to that\n    user's identity, tenant and permissions. They are not interchangeable.\noverview: >-\n  Amperity APIs authenticate with a JWT bearer access token. An administrator creates an API key\n  (a synthetic identity bound to the tenant) under Settings\
  \ > Security > API keys, granting it the\n  DataGrid Operator role. The API key's client_id/client_secret are exchanged for a short-lived\n  access token via the OAuth2 client-credentials token endpoint. All API requests then send the\n  token in the Authorization header, plus a tenant identifier header and a date-based api-version\n  header.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.amperity.com/api/v0/oauth2/token\n    grant_type: client_credentials\n    request_content_type: application/x-www-form-urlencoded\n    request_params: [client_id, client_secret]\n    token_response:\n      access_token: string\n      token_type: Bearer\n      expires_in: 3600\n    scopes: {}\n  sources: [https://docs.amperity.com/api/authentication.html]\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_via: 'Authorization: Bearer ${access-token}'\n  sources: [https://docs.amperity.com/api/authentication.html]\n\
  required_headers:\n- name: Authorization\n  value: 'Bearer ${access-token}'\n  apis: [Amperity API, Profile API, Streaming API]\n- name: amperity-tenant\n  value: '{tenant-id}'\n  apis: [Profile API]\n- name: X-Amperity-Tenant\n  value: '{tenant-name}'\n  apis: [Amperity API, Streaming API]\n- name: api-version\n  value: 'YYYY-MM-DD (e.g. 2024-04-01 for Amperity API, 2025-07-31 for Profile API)'\n  apis: [Amperity API, Profile API]\ntoken_lifecycle:\n  format: JWT\n  expiry: 'expires_in seconds (default 3600); UI-generated tokens expire after a configured number of days'\n  refresh: 'no refresh-grant flow; regenerate via client-credentials exchange or the UI'\n  key_rotation: 'rotating an API key mints a new secret; previously issued tokens remain valid for 30 days (deposed state) before becoming invalid'\nnotes:\n- API keys are managed under Settings > Security and require the API key administration policy.\n- The Streaming API uses a self-managed Streaming Ingest JWT token generated\
  \ in the UI.\nmcp_oauth:\n  surface: https://mcp.amperity.com\n  method: probed\n  source: well-known/amperity-oauth-authorization-server.json\n  checked: '2026-08-13'\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  issuer: https://mcp.amperity.com\n  authorization_endpoint: https://mcp.amperity.com/authorize\n  token_endpoint: https://mcp.amperity.com/oauth/token\n  registration_endpoint: https://mcp.amperity.com/oauth/register\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code]\n  token_endpoint_auth_methods_supported: [none]\n  bearer_methods_supported: [header]\n  dynamic_client_registration: true\n  published_client_id: nwbd0MGCyh1VysmYQM05UoDXIuVPdGEs\n  published_client_id_note: >-\n    Amperity publishes this public client id verbatim in its Claude setup documentation for use when\n    adding the custom connector. It is a public client (token_endpoint_auth_methods_supported: [none]),\n    not a secret.\n  challenge:\n    observed: 'HTTP\
  \ 401 on POST tools/list'\n    www_authenticate: 'Bearer resource_metadata=\"https://mcp.amperity.com/.well-known/oauth-protected-resource\"'\n    note: 'Full RFC 9728 protected-resource handshake - the 401 points a client at its own metadata.'\n  scopes:\n    published: []\n    note: >-\n      No scopes_supported is advertised in the authorization-server metadata and no scope reference\n      page exists. Authorization is carried by the calling user's Amperity policies and by the\n      per-session MCP safety mode, not by OAuth scopes. This is why no scopes/ artifact is emitted for\n      Amperity - there is no scope surface to record.\n  authorization_model:\n    basis: 'The calling user''s Amperity identity, tenant access and policies.'\n    session_guardrail: 'Per-session MCP safety mode (strict / confirm / unrestricted).'\n    ref: mcp/amperity-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/authentication/amperity-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Enterprise
- Customer Data Platform
- CDP
- Identity Resolution
- Customer 360
- Marketing
- Data
- Profiles
- Analytics
- MCP
- Agents
- Retail
- Identity
---
