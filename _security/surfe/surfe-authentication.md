---
api_key_in:
- header
api_specs:
- filename: surfe-account-api-openapi.yml
  format: yaml
  label: Surfe Account API
  slug: surfe-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-account-api-openapi.yml
- filename: surfe-companies-api-openapi.yml
  format: yaml
  label: Surfe Companies API
  slug: surfe-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-companies-api-openapi.yml
- filename: surfe-people-api-openapi.yml
  format: yaml
  label: Surfe People API
  slug: surfe-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-people-api-openapi.yml
- filename: surfe-recommendations-api-openapi.yml
  format: yaml
  label: Surfe Recommendations API
  slug: surfe-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-recommendations-api-openapi.yml
auth_types:
- http
- oauth2
description: 'Surfe runs two authentication surfaces off ONE credential. The REST API takes the Surfe API key directly as an HTTP bearer token. The hosted MCP server and the official `surfer` CLI wrap that same key in OAuth 2.0 authorization code + PKCE: you paste the key once at Surfe''s sign-in page and the client holds a managed token instead of the raw key. API keys are per-user and each user may hold exactly one at a time.'
kind: authentication
layout: security
method: searched
name: Surfe Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Surfe secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Surfe
provider_slug: surfe
scheme_count: 3
schemes:
- description: 'Surfe API key issued from the Surfe dashboard, sent as `Authorization: Bearer {api-key}`. Required on every request to every endpoint — the API host answers unauthenticated requests to any path with 401 {"code":401,"message":"Missing or wrong API key"}.'
  key_management: https://app.surfe.com/api-settings
  keys_per_user: 1
  name: bearerAuth
  rotation: Surfe's guidance is to delete a suspected-compromised key immediately and create a new one from the dashboard. No programmatic rotation endpoint is documented.
  scheme: bearer
  sources:
  - openapi/surfe-openapi.yml
  - https://developers.surfe.com/api-key
  surface: rest
  type: http
- description: OAuth 2.0 for the hosted MCP server at https://mcp.eu.surfe.com/mcp. Advertised via RFC 8414 authorization server metadata and RFC 9728 protected resource metadata; the client exchanges the user's Surfe API key at Surfe's sign-in page for a managed token.
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.eu.surfe.com/authorize
    bearer_methods:
    - header
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    issuer: https://mcp.eu.surfe.com/
    registrationUrl: https://mcp.eu.surfe.com/register
    revocationUrl: https://mcp.eu.surfe.com/revoke
    scopes:
      surfe: Access to the Surfe MCP tool surface (the only scope advertised).
    tokenUrl: https://mcp.eu.surfe.com/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: surfeMcpOAuth
  sources:
  - well-known/surfe-oauth-authorization-server.json
  - well-known/surfe-oauth-protected-resource.json
  - https://developers.surfe.com/mcp
  surface: mcp
  type: oauth2
- description: '`surfer login` opens the browser and runs OAuth 2.0 + PKCE against Surfe''s auth host, storing tokens at ~/.surfer/tokens.json with mode 0600. For non-interactive use (CI, agents) the CLI accepts the raw API key in the SURFE_API_KEY environment variable and skips the OAuth flow entirely.'
  flows:
  - authHost: https://eu.prod.surfe.com
    code_challenge_methods:
    - S256
    flow: authorizationCode
  name: surferCliOAuth
  non_interactive_credential: SURFE_API_KEY
  sources:
  - https://github.com/Surfe/surfer
  - https://raw.githubusercontent.com/surfe/surfer/main/AGENTS.md
  surface: cli
  token_storage: ~/.surfer/tokens.json (0600)
  type: oauth2
slug: surfe-authentication
source_filename: surfe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/surfe-openapi.yml\ndocs: https://developers.surfe.com/api-key\ndescription: >-\n  Surfe runs two authentication surfaces off ONE credential. The REST API takes\n  the Surfe API key directly as an HTTP bearer token. The hosted MCP server and\n  the official `surfer` CLI wrap that same key in OAuth 2.0 authorization code\n  + PKCE: you paste the key once at Surfe's sign-in page and the client holds a\n  managed token instead of the raw key. API keys are per-user and each user may\n  hold exactly one at a time.\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: rest\n  description: >-\n    Surfe API key issued from the Surfe dashboard, sent as\n    `Authorization: Bearer {api-key}`. Required on every request to every\n    endpoint — the API host answers unauthenticated requests to any path\
  \ with\n    401 {\"code\":401,\"message\":\"Missing or wrong API key\"}.\n  key_management: https://app.surfe.com/api-settings\n  keys_per_user: 1\n  rotation: >-\n    Surfe's guidance is to delete a suspected-compromised key immediately and\n    create a new one from the dashboard. No programmatic rotation endpoint is\n    documented.\n  sources:\n  - openapi/surfe-openapi.yml\n  - https://developers.surfe.com/api-key\n- name: surfeMcpOAuth\n  type: oauth2\n  surface: mcp\n  description: >-\n    OAuth 2.0 for the hosted MCP server at https://mcp.eu.surfe.com/mcp.\n    Advertised via RFC 8414 authorization server metadata and RFC 9728 protected\n    resource metadata; the client exchanges the user's Surfe API key at Surfe's\n    sign-in page for a managed token.\n  flows:\n  - flow: authorizationCode\n    issuer: https://mcp.eu.surfe.com/\n    authorizationUrl: https://mcp.eu.surfe.com/authorize\n    tokenUrl: https://mcp.eu.surfe.com/token\n    registrationUrl: https://mcp.eu.surfe.com/register\n\
  \    revocationUrl: https://mcp.eu.surfe.com/revoke\n    scopes:\n      surfe: Access to the Surfe MCP tool surface (the only scope advertised).\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    bearer_methods: [header]\n  dynamic_client_registration: true\n  sources:\n  - well-known/surfe-oauth-authorization-server.json\n  - well-known/surfe-oauth-protected-resource.json\n  - https://developers.surfe.com/mcp\n- name: surferCliOAuth\n  type: oauth2\n  surface: cli\n  description: >-\n    `surfer login` opens the browser and runs OAuth 2.0 + PKCE against Surfe's\n    auth host, storing tokens at ~/.surfer/tokens.json with mode 0600. For\n    non-interactive use (CI, agents) the CLI accepts the raw API key in the\n    SURFE_API_KEY environment variable and skips the OAuth flow entirely.\n  flows:\n  - flow: authorizationCode\n    authHost: https://eu.prod.surfe.com\n \
  \   code_challenge_methods: [S256]\n  non_interactive_credential: SURFE_API_KEY\n  token_storage: ~/.surfer/tokens.json (0600)\n  sources:\n  - https://github.com/Surfe/surfer\n  - https://raw.githubusercontent.com/surfe/surfer/main/AGENTS.md\nunauthenticated_response:\n  status: 401\n  body: '{\"code\":401,\"message\":\"Missing or wrong API key\"}'\n  observed: '2026-08-13'\n  observed_on: https://api.surfe.com/\nnotes: >-\n  No OpenID Connect discovery document is served on any Surfe host\n  (/.well-known/openid-configuration 404s on mcp.eu.surfe.com,\n  developers.surfe.com, www.surfe.com and app.surfe.com; 401 on api.surfe.com).\n  The REST API declares no OAuth scopes — scoping exists only on the MCP\n  surface, where a single `surfe` scope is advertised.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/authentication/surfe-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- B2B Data
- Contact Data
- Sales Intelligence
- Enrichment
- Lead Generation
- CRM
- Prospecting
---
