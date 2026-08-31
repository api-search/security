---
api_key_in:
- header
api_specs:
- filename: 2x-alignment-api-openapi.yml
  format: yaml
  label: 2X Alignment API
  slug: 2x-alignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-alignment-api-openapi.yml
- filename: 2x-api-keys-api-openapi.yml
  format: yaml
  label: 2X API Keys API
  slug: 2x-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-api-keys-api-openapi.yml
- filename: 2x-clients-api-openapi.yml
  format: yaml
  label: 2X Clients API
  slug: 2x-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-clients-api-openapi.yml
- filename: 2x-documentation-api-openapi.yml
  format: yaml
  label: 2X Documentation API
  slug: 2x-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-documentation-api-openapi.yml
- filename: 2x-health-api-openapi.yml
  format: yaml
  label: 2X Health API
  slug: 2x-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-health-api-openapi.yml
- filename: 2x-portfolios-api-openapi.yml
  format: yaml
  label: 2X Portfolios API
  slug: 2x-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-portfolios-api-openapi.yml
- filename: 2x-root-api-openapi.yml
  format: yaml
  label: 2X Root API
  slug: 2x-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-root-api-openapi.yml
- filename: 2x-status-api-openapi.yml
  format: yaml
  label: 2X Status API
  slug: 2x-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-status-api-openapi.yml
- filename: 2x-streams-api-openapi.yml
  format: yaml
  label: 2X Streams API
  slug: 2x-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-streams-api-openapi.yml
- filename: 2x-topics-api-openapi.yml
  format: yaml
  label: 2X Topics API
  slug: 2x-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-topics-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: 2X Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 2X secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 2X
provider_slug: 2x
scheme_count: 2
schemes:
- applies_to: https://api.knownwell.com/ci/v1
  description: Static per-customer API key. Sent on every request as X-API-Key. A missing key returns HTTP 401 with body {"detail":"API key is required. Provide it in the X-API-Key header."} (observed 2026-08-13). Keys are issued and revoked through the /v1/api-keys operations, which are themselves protected by a separate `authorization` header parameter, so there is no anonymous self-serve key issuance.
  in: header
  key_management:
    create: create_api_key_v1_api_keys_post
    expiry_field: expires_days
    list: list_api_keys_v1_api_keys_get
    revoke: revoke_api_key_v1_api_keys__key_id__delete
    scope_field: scope
    scoped: true
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/2x-knownwell-openapi.json
  type: apiKey
- applies_to: https://mcp.knownwell.com/mcp
  bearer_methods:
  - header
  code_challenge_methods:
  - S256
  description: OAuth 2.1 authorization-code flow with mandatory PKCE, protecting the remote MCP endpoint. Supports dynamic client registration, so an MCP client can onboard without a pre-provisioned client_id.
  flows:
  - authorizationUrl: https://mcp.knownwell.com/authorize
    flow: authorizationCode
    scopes:
      knownwell.read: Read access to Knownwell commercial-intelligence data
    tokenUrl: https://mcp.knownwell.com/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.knownwell.com/
  method: probed
  name: KnownwellMCPOAuth
  registration_endpoint: https://mcp.knownwell.com/register
  revocation_endpoint: https://mcp.knownwell.com/revoke
  sources:
  - well-known/2x-oauth-authorization-server.json
  - well-known/2x-oauth-protected-resource.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: 2x-authentication
source_filename: 2x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/2x-knownwell-openapi.json\ndocs: https://api.knownwell.com/docs\nnote: >-\n  2X's API surface (acquired with Knownwell in June 2026) uses two different auth models on\n  two different hosts. The REST commercial-intelligence API on api.knownwell.com takes a\n  static API key in an X-API-Key header. The remote MCP server on mcp.knownwell.com takes an\n  OAuth 2.1 bearer token and publishes full RFC 8414 / RFC 9728 discovery. The OpenAPI\n  declares only the first of these, so the OAuth model below was probed from the live\n  discovery documents rather than derived from the spec.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  applies_to: https://api.knownwell.com/ci/v1\n  sources:\n  - openapi/2x-knownwell-openapi.json\n  description: >-\n    Static per-customer API key.\
  \ Sent on every request as X-API-Key. A missing key returns\n    HTTP 401 with body {\"detail\":\"API key is required. Provide it in the X-API-Key header.\"}\n    (observed 2026-08-13). Keys are issued and revoked through the /v1/api-keys operations,\n    which are themselves protected by a separate `authorization` header parameter, so there\n    is no anonymous self-serve key issuance.\n  key_management:\n    create: create_api_key_v1_api_keys_post\n    list: list_api_keys_v1_api_keys_get\n    revoke: revoke_api_key_v1_api_keys__key_id__delete\n    scoped: true\n    scope_field: scope\n    expiry_field: expires_days\n- name: KnownwellMCPOAuth\n  type: oauth2\n  applies_to: https://mcp.knownwell.com/mcp\n  method: probed\n  sources:\n  - well-known/2x-oauth-authorization-server.json\n  - well-known/2x-oauth-protected-resource.json\n  description: >-\n    OAuth 2.1 authorization-code flow with mandatory PKCE, protecting the remote MCP\n    endpoint. Supports dynamic client registration,\
  \ so an MCP client can onboard without a\n    pre-provisioned client_id.\n  issuer: https://mcp.knownwell.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.knownwell.com/authorize\n    tokenUrl: https://mcp.knownwell.com/token\n    scopes:\n      knownwell.read: Read access to Knownwell commercial-intelligence data\n  registration_endpoint: https://mcp.knownwell.com/register\n  revocation_endpoint: https://mcp.knownwell.com/revoke\n  code_challenge_methods: [S256]\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  bearer_methods: [header]\nanonymous_surfaces:\n- url: https://api.knownwell.com/openapi.json\n  note: the OpenAPI document itself is served without authentication\n- url: https://api.knownwell.com/health\n  note: health check is anonymous\n- url: https://2x.com/wp-json/\n  note: >-\n    the corporate site's WordPress REST API is anonymously readable; WordPress application\n\
  \    passwords are the documented write-side auth but no anonymous write is exposed\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://api.knownwell.com/v1/clients\n    status: 401\n    body: '{\"detail\":\"API key is required. Provide it in the X-API-Key header.\"}'\n  - url: https://mcp.knownwell.com/mcp\n    status: 401\n    www_authenticate: Bearer error=\"invalid_token\"\n  - url: https://mcp.knownwell.com/.well-known/oauth-authorization-server\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/authentication/2x-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Marketing
- Marketing as a Service
- B2B
- MarTech
- Marketing Operations
- Consulting
- Artificial Intelligence
- Go-To-Market
- Revenue Operations
- Commercial Intelligence
- Customer Success
- Agentic AI
- Demand Generation
---
