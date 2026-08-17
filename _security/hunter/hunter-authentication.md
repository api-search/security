---
api_key_in:
- header
- query
api_specs:
- filename: hunter-account-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: hunter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-account-api-openapi.yml
- filename: hunter-campaigns-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: hunter-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-campaigns-api-openapi.yml
- filename: hunter-combined-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Combined Enrichment API
  slug: hunter-combined-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-combined-enrichment-api-openapi.yml
- filename: hunter-company-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Company Enrichment API
  slug: hunter-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-company-enrichment-api-openapi.yml
- filename: hunter-discover-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: hunter-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-discover-api-openapi.yml
- filename: hunter-domain-search-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: hunter-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-domain-search-api-openapi.yml
- filename: hunter-email-count-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: hunter-email-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-count-api-openapi.yml
- filename: hunter-email-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Email Enrichment API
  slug: hunter-email-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-enrichment-api-openapi.yml
- filename: hunter-email-finder-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: hunter-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-finder-api-openapi.yml
- filename: hunter-email-verifier-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: hunter-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-verifier-api-openapi.yml
- filename: hunter-leads-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: hunter-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-api-openapi.yml
- filename: hunter-leads-lists-api-openapi.yml
  format: yaml
  label: Hunter Leads Lists API
  slug: hunter-leads-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-lists-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: Hunter authenticates every call with a single account API key, accepted in three interchangeable positions. The OpenAPI declares all three. Separately — and documented nowhere in the API reference — hunter.io runs a full OAuth 2.1 authorization server, discovered by probing RFC 8414 metadata; it is what the remote MCP server at mcp.hunter.io delegates to via RFC 9728 protected-resource metadata.
kind: authentication
layout: security
method: searched
name: Hunter Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Hunter secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Hunter
provider_slug: hunter
scheme_count: 4
schemes:
- description: API key passed as a query parameter. This is the form used throughout Hunter's own examples.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/_original/hunter-api-openapi.yml
  - https://hunter.io/api-documentation/v2#authentication
  type: apiKey
- description: API key passed via the X-API-KEY header. Also accepted by the remote MCP server.
  in: header
  name: apiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/_original/hunter-api-openapi.yml
  - https://hunter.io/api-documentation/v2#authentication
  type: apiKey
- description: API key passed as a Bearer token in the Authorization header. Note this is the API key itself, not an OAuth access token. Also accepted by the remote MCP server.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/hunter-api-openapi.yml
  - https://hunter.io/api-documentation/v2#authentication
  type: http
- artifact: scopes/hunter-scopes.yml
  authorizationUrl: https://hunter.io/oauth/authorize
  description: OAuth 2.1-shaped authorization server at https://hunter.io. Not declared in the OpenAPI and not written up in the API reference; discovered from discovery metadata. Supports authorization code with PKCE S256, client credentials and refresh tokens, plus RFC 7591 dynamic client registration and the public-client token_endpoint_auth_method "none".
  introspectionUrl: https://hunter.io/oauth/introspect
  issuer: https://hunter.io
  jwksUri: https://hunter.io/oauth/discovery/keys
  name: oauth2
  registrationUrl: https://hunter.io/oauth/register
  revocationUrl: https://hunter.io/oauth/revoke
  scopes:
  - read
  - write
  sources:
  - https://hunter.io/.well-known/oauth-authorization-server
  - https://hunter.io/.well-known/openid-configuration
  - https://mcp.hunter.io/.well-known/oauth-protected-resource
  tokenUrl: https://hunter.io/oauth/token
  type: oauth2
  userinfoUrl: https://hunter.io/oauth/userinfo
slug: hunter-authentication
source_filename: hunter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/hunter-api-openapi.yml\ndocs: https://hunter.io/api-documentation/v2#authentication\ndescription: >-\n  Hunter authenticates every call with a single account API key, accepted in three interchangeable\n  positions. The OpenAPI declares all three. Separately — and documented nowhere in the API\n  reference — hunter.io runs a full OAuth 2.1 authorization server, discovered by probing RFC 8414\n  metadata; it is what the remote MCP server at mcp.hunter.io delegates to via RFC 9728\n  protected-resource metadata.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a query parameter. This is the form used throughout Hunter's own examples.\n  sources:\n  - openapi/_original/hunter-api-openapi.yml\n\
  \  - https://hunter.io/api-documentation/v2#authentication\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key passed via the X-API-KEY header. Also accepted by the remote MCP server.\n  sources:\n  - openapi/_original/hunter-api-openapi.yml\n  - https://hunter.io/api-documentation/v2#authentication\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key passed as a Bearer token in the Authorization header. Note this is the API key itself,\n    not an OAuth access token. Also accepted by the remote MCP server.\n  sources:\n  - openapi/_original/hunter-api-openapi.yml\n  - https://hunter.io/api-documentation/v2#authentication\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.1-shaped authorization server at https://hunter.io. Not declared in the OpenAPI and not\n    written up in the API reference; discovered from discovery metadata. Supports authorization\n    code with PKCE S256, client credentials\
  \ and refresh tokens, plus RFC 7591 dynamic client\n    registration and the public-client token_endpoint_auth_method \"none\".\n  issuer: https://hunter.io\n  authorizationUrl: https://hunter.io/oauth/authorize\n  tokenUrl: https://hunter.io/oauth/token\n  revocationUrl: https://hunter.io/oauth/revoke\n  introspectionUrl: https://hunter.io/oauth/introspect\n  userinfoUrl: https://hunter.io/oauth/userinfo\n  jwksUri: https://hunter.io/oauth/discovery/keys\n  registrationUrl: https://hunter.io/oauth/register\n  scopes: [read, write]\n  artifact: scopes/hunter-scopes.yml\n  sources:\n  - https://hunter.io/.well-known/oauth-authorization-server\n  - https://hunter.io/.well-known/openid-configuration\n  - https://mcp.hunter.io/.well-known/oauth-protected-resource\nkey_management:\n  self_serve: true\n  location: Hunter dashboard\n  api: 'API-key management is exposed through the MCP server (List-API-Keys, Create-API-Key, Delete-API-Key) and the docs'' API keys section, but not through the\
  \ captured v2 OpenAPI.'\n  rotation_policy: null\ntest_credential:\n  key: test-api-key\n  artifact: sandbox/hunter-sandbox.yml\nfindings:\n- id: jwks-uri-500\n  detail: The advertised jwks_uri https://hunter.io/oauth/discovery/keys returned HTTP 500 when probed on 2026-08-13.\n- id: oauth-undocumented\n  detail: >-\n    A production OAuth/OIDC authorization server exists but appears in no human documentation.\n    Integrators can only find it by reading the well-known discovery documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/authentication/hunter-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
---
