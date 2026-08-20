---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Enigma Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Enigma secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Enigma
provider_slug: enigma
scheme_count: 3
schemes:
- applies_to:
  - Enigma GraphQL Data API (https://api.enigma.com/graphql)
  - Enigma KYB REST API (https://api.enigma.com/v2/kyb/)
  - Enigma Screening API (https://api.enigma.com/evaluation/sanctions/)
  in: header
  name: apiKey
  notes: Each request must include the x-api-key header. Keys are managed via the Enigma Console (https://console.enigma.com/) or an account representative. There is no test key, no key prefix convention, and no documented rotation or expiry policy.
  observed_401:
    graphql: '{"error_message":"Missing or invalid API key","error_code":"UNAUTHORIZED","retryable":false}'
    kyb: '{"error":true,"message":"Unauthorized"}'
    observed_at: '2026-08-14'
  parameter_name: x-api-key
  type: apiKey
- applies_to:
  - Enigma Screening API (https://api.enigma.com/evaluation/sanctions/)
  in: header
  name: accountName
  notes: The Screening API requires a second header, Account-Name, alongside x-api-key on every documented request. The GraphQL and KYB APIs do not.
  parameter_name: Account-Name
  required: true
  type: apiKey
- applies_to:
  - Enigma MCP server (https://mcp.enigma.com/mcp)
  discovery:
    authorization_server_metadata: https://mcp.enigma.com/.well-known/oauth-authorization-server
    openid_configuration: null
    protected_resource_metadata: https://mcp.enigma.com/.well-known/oauth-protected-resource
  dynamic_client_registration: https://oauth.enigma.com/register
  flows:
  - authorizationUrl: https://oauth.enigma.com/authorize
    flow: authorizationCode
    pkce: S256 (required)
    tokenUrl: https://oauth.enigma.com/token
  grant_types:
  - authorization_code
  - refresh_token
  identity_provider: Amazon Cognito (us-east-1_00OC0VOa2)
  introspection_endpoint: https://oauth.enigma.com/introspect
  issuer: https://oauth.enigma.com
  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_00OC0VOa2/.well-known/jwks.json
  name: oauth2
  notes: 'Discovery is fully machine-readable and RFC-conformant: an unauthenticated call gets a 401 with WWW-Authenticate naming the protected-resource document, which names the authorization server, which advertises registration/authorize/token/revoke/introspect. An agent can complete the whole handshake without reading a docs page. Scope granularity is the weak point — only `openid` is advertised, so entitlement is enforced by plan and per-tool rate limit rather than by scope.'
  revocation_endpoint: https://oauth.enigma.com/revoke
  scopes:
  - openid
  see: scopes/enigma-scopes.yml
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
  version: '2.1'
slug: enigma-authentication
source_filename: enigma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://documentation.enigma.com/guides/graphql/api\ndocs:\n- https://documentation.enigma.com/guides/graphql/api\n- https://documentation.enigma.com/screening/api\n- https://documentation.enigma.com/guides/ai-mcp\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Two disjoint models: a static API key for all three HTTP APIs, and OAuth 2.1 for the\n    remote MCP server. There is no way to call the HTTP APIs with an OAuth token, and no\n    way to call MCP with an API key.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to:\n  - Enigma GraphQL Data API (https://api.enigma.com/graphql)\n  - Enigma KYB REST API (https://api.enigma.com/v2/kyb/)\n  - Enigma Screening API (https://api.enigma.com/evaluation/sanctions/)\n  observed_401:\n    graphql: '{\"error_message\":\"Missing or invalid API key\",\"error_code\"\
  :\"UNAUTHORIZED\",\"retryable\":false}'\n    kyb: '{\"error\":true,\"message\":\"Unauthorized\"}'\n    observed_at: '2026-08-14'\n  notes: >-\n    Each request must include the x-api-key header. Keys are managed via the Enigma\n    Console (https://console.enigma.com/) or an account representative. There is no test\n    key, no key prefix convention, and no documented rotation or expiry policy.\n- name: accountName\n  type: apiKey\n  in: header\n  parameter_name: Account-Name\n  applies_to:\n  - Enigma Screening API (https://api.enigma.com/evaluation/sanctions/)\n  required: true\n  notes: >-\n    The Screening API requires a second header, Account-Name, alongside x-api-key on every\n    documented request. The GraphQL and KYB APIs do not.\n- name: oauth2\n  type: oauth2\n  version: '2.1'\n  applies_to:\n  - Enigma MCP server (https://mcp.enigma.com/mcp)\n  issuer: https://oauth.enigma.com\n  identity_provider: Amazon Cognito (us-east-1_00OC0VOa2)\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://oauth.enigma.com/authorize\n    tokenUrl: https://oauth.enigma.com/token\n    pkce: S256 (required)\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_basic]\n  dynamic_client_registration: https://oauth.enigma.com/register\n  revocation_endpoint: https://oauth.enigma.com/revoke\n  introspection_endpoint: https://oauth.enigma.com/introspect\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_00OC0VOa2/.well-known/jwks.json\n  scopes: [openid]\n  discovery:\n    authorization_server_metadata: https://mcp.enigma.com/.well-known/oauth-authorization-server\n    protected_resource_metadata: https://mcp.enigma.com/.well-known/oauth-protected-resource\n    openid_configuration: null\n  notes: >-\n    Discovery is fully machine-readable and RFC-conformant: an unauthenticated call gets a\n    401 with WWW-Authenticate naming the protected-resource document, which names the\n    authorization server, which\
  \ advertises registration/authorize/token/revoke/introspect.\n    An agent can complete the whole handshake without reading a docs page. Scope\n    granularity is the weak point — only `openid` is advertised, so entitlement is\n    enforced by plan and per-tool rate limit rather than by scope.\n  see: scopes/enigma-scopes.yml\nsso:\n  console: https://documentation.enigma.com/console/sso-configuration\n  note: The Enigma Console supports customer SSO configuration (documented; provider-side setup).\nx-evidence:\n  fetched: '2026-08-14'\n  probes:\n  - {url: 'https://api.enigma.com/graphql', method: POST, http_status: 401}\n  - {url: 'https://api.enigma.com/v2/kyb/', method: POST, http_status: 401}\n  - {url: 'https://mcp.enigma.com/mcp', method: POST, http_status: 401}\n  - {url: 'https://mcp.enigma.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://mcp.enigma.com/.well-known/oauth-protected-resource', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigma/refs/heads/main/authentication/enigma-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Business Data
- Identity Resolution
- KYB
- Compliance
- Fraud
- GraphQL
- Data Enrichment
- Financial-Services
- MCP
- Sanctions Screening
- Agent Skills
---
