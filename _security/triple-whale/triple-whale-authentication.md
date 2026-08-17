---
api_key_in:
- header
api_specs:
- filename: triple-whale-api-keys-api-openapi.yml
  format: yaml
  label: Triple Whale API Keys API
  slug: triple-whale-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-api-keys-api-openapi.yml
- filename: triple-whale-compliance-api-openapi.yml
  format: yaml
  label: Triple Whale Compliance API
  slug: triple-whale-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-compliance-api-openapi.yml
- filename: triple-whale-data-in-api-openapi.yml
  format: yaml
  label: Triple Whale Data In API
  slug: triple-whale-data-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-data-in-api-openapi.yml
- filename: triple-whale-data-out-api-openapi.yml
  format: yaml
  label: Triple Whale Data Out API
  slug: triple-whale-data-out-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-data-out-api-openapi.yml
- filename: triple-whale-bi-benchmarks-openapi.json
  format: json
  label: Triple Whale Benchmarks API
  slug: triple-whale-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-bi-benchmarks-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Triple Whale Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Triple Whale secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Triple Whale
provider_slug: triple-whale
scheme_count: 2
schemes:
- constraints:
  - Shopify session JWTs and other token types are explicitly not accepted.
  - Keys are bound to the user who created them; if that user loses workspace access, the key stops working.
  - Separate keys are recommended per environment (production, testing, development).
  failure_mode:
    causes:
    - missing header
    - revoked or expired key
    - missing scope
    - wrong token type
    status: 401
  in: header
  issuance:
    console: https://app.triplewhale.com/api-keys
    path: Data > APIs > Generate
    revocable: true
    revocation_irreversible: true
    shown_once: true
  name: apiKeyAuth
  parameter: x-api-key
  scoped: true
  scopes: scopes/triple-whale-scopes.yml
  sources:
  - openapi/triple-whale-api-keys-api-openapi.yml
  - openapi/triple-whale-compliance-api-openapi.yml
  - openapi/triple-whale-data-in-api-openapi.yml
  - openapi/triple-whale-data-out-api-openapi.yml
  surface: rest
  type: apiKey
  verification:
    note: Returns the scopes attached to the presented key.
    operation: validate-your-triple-whale-api-key
    request: GET https://api.triplewhale.com/api/v2/users/api-keys/me
- bearer_methods:
  - header
  discovery:
  - https://mcp.triplewhale.com/.well-known/oauth-authorization-server
  - https://mcp.triplewhale.com/.well-known/oauth-protected-resource
  files:
  - well-known/triple-whale-oauth-authorization-server.json
  - well-known/triple-whale-oauth-protected-resource.json
  flows:
  - authorizationUrl: https://mcp.triplewhale.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://mcp.triplewhale.com/register
    scopes:
    - moby:read
    - offline
    - offline_access
    tokenUrl: https://mcp.triplewhale.com/token
  method: probed
  name: mcpOAuth
  note: 'Public client with dynamic client registration and PKCE; no client secret (token_endpoint_auth_methods is ["none"]). An "MCP: Read" API key is the alternative, non-OAuth path documented for the same server.'
  probed: '2026-08-13'
  resource: https://mcp.triplewhale.com/sse
  surface: mcp
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: triple-whale-authentication
source_filename: triple-whale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource:\n- https://triplewhale.readme.io/reference/creating-and-managing-triple-whale-api-keys\n- https://triplewhale.readme.io/reference/troubleshooting-common-triple-whale-api-errors\n- https://mcp.triplewhale.com/.well-known/oauth-authorization-server\nderived_from:\n- openapi/triple-whale-api-keys-api-openapi.yml\n- openapi/triple-whale-compliance-api-openapi.yml\n- openapi/triple-whale-data-in-api-openapi.yml\n- openapi/triple-whale-data-out-api-openapi.yml\ndocs: https://triplewhale.readme.io/reference/creating-and-managing-triple-whale-api-keys\n\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    The REST API is API-key only — every published operation is secured by\n    apiKeyAuth (x-api-key) and no OpenAPI declares an oauth2 scheme. OAuth 2.1\n    appears only on the hosted MCP server, which is a separate surface.\n\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter: x-api-key\n  surface: rest\n  sources:\n  - openapi/triple-whale-api-keys-api-openapi.yml\n  - openapi/triple-whale-compliance-api-openapi.yml\n  - openapi/triple-whale-data-in-api-openapi.yml\n  - openapi/triple-whale-data-out-api-openapi.yml\n  issuance:\n    console: https://app.triplewhale.com/api-keys\n    path: Data > APIs > Generate\n    shown_once: true\n    revocable: true\n    revocation_irreversible: true\n  scoped: true\n  scopes: scopes/triple-whale-scopes.yml\n  verification:\n    operation: validate-your-triple-whale-api-key\n    request: GET https://api.triplewhale.com/api/v2/users/api-keys/me\n    note: Returns the scopes attached to the presented key.\n  constraints:\n  - Shopify session JWTs and other token types are explicitly not accepted.\n  - >-\n    Keys are bound to the user who created them; if that user loses workspace\n    access, the key stops working.\n  - Separate keys are recommended per environment (production, testing, development).\n\
  \  failure_mode:\n    status: 401\n    causes: [missing header, revoked or expired key, missing scope, wrong token type]\n\n- name: mcpOAuth\n  type: oauth2\n  surface: mcp\n  resource: https://mcp.triplewhale.com/sse\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.triplewhale.com/authorize\n    tokenUrl: https://mcp.triplewhale.com/token\n    registrationUrl: https://mcp.triplewhale.com/register\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    scopes: [moby:read, offline, offline_access]\n  token_endpoint_auth_methods: [none]\n  bearer_methods: [header]\n  discovery:\n  - https://mcp.triplewhale.com/.well-known/oauth-authorization-server\n  - https://mcp.triplewhale.com/.well-known/oauth-protected-resource\n  files:\n  - well-known/triple-whale-oauth-authorization-server.json\n  - well-known/triple-whale-oauth-protected-resource.json\n  method: probed\n  probed: '2026-08-13'\n  note: >-\n    Public client with dynamic\
  \ client registration and PKCE; no client secret\n    (token_endpoint_auth_methods is [\"none\"]). An \"MCP: Read\" API key is the\n    alternative, non-OAuth path documented for the same server.\n\nanonymous_surfaces:\n- endpoint: GET https://api.triplewhale.com/api/v2/bi/avg\n  auth: none\n  spec: openapi/triple-whale-bi-benchmarks-openapi.json\n  evidence: >-\n    https://api.triplewhale.com/.well-known/ai-plugin.json declares auth type\n    \"none\" for this API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/authentication/triple-whale-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- E-commerce
- Analytics
- Attribution
- Shopify
- Pixel Tracking
- ROAS
- DTC
- Marketing
---
