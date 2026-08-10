---
api_key_in:
- header
api_specs:
- filename: zillapi-account-api-openapi.yml
  format: yaml
  label: Zillapi Account API
  slug: zillapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-account-api-openapi.yml
- filename: zillapi-buildings-api-openapi.yml
  format: yaml
  label: Zillapi Buildings API
  slug: zillapi-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-buildings-api-openapi.yml
- filename: zillapi-jobs-api-openapi.yml
  format: yaml
  label: Zillapi Jobs API
  slug: zillapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-jobs-api-openapi.yml
- filename: zillapi-listings-api-openapi.yml
  format: yaml
  label: Zillapi Listings API
  slug: zillapi-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-listings-api-openapi.yml
- filename: zillapi-properties-api-openapi.yml
  format: yaml
  label: Zillapi Properties API
  slug: zillapi-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-properties-api-openapi.yml
- filename: zillapi-search-api-openapi.yml
  format: yaml
  label: Zillapi Search API
  slug: zillapi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-search-api-openapi.yml
- filename: zillapi-webhooks-api-openapi.yml
  format: yaml
  label: Zillapi Webhooks API
  slug: zillapi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zillapi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zillapi secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zillapi
provider_slug: zillapi
scheme_count: 2
schemes:
- bearerFormat: API key (zk_*)
  key_format:
    body: 43 characters, URL-safe base64 of 32 random bytes
    prefix: zk_
    total_length: 46
  management_url: https://zillapi.com/app/keys/
  name: bearerAuth
  rotation:
    documented: true
    procedure:
    - Create a new key in the dashboard
    - Roll it into the environment
    - Confirm traffic on the new key under Usage
    - Revoke the old key
    revocation: immediate — calls on a revoked key return 401 invalid_api_key within seconds
  scheme: bearer
  signup_url: https://zillapi.com/signup
  sources:
  - openapi/zillapi-openapi-original.json
  storage: Plaintext shown once at creation; provider states it stores only the SHA-256 hash and cannot recover the original.
  type: http
- dynamic_client_registration:
    endpoint: https://api.zillapi.com/oauth/register
    standard: RFC 7591
    supported: true
  flows:
  - authorizationUrl: https://api.zillapi.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    pkce_required: true
    registrationUrl: https://api.zillapi.com/oauth/register
    revocationUrl: https://api.zillapi.com/oauth/revoke
    scopes:
      mcp:access: Access the Zillapi MCP server and the /v1 REST surface
    tokenUrl: https://api.zillapi.com/oauth/token
    token_endpoint_auth_methods:
    - none
  intended_for: remote-MCP connectors (e.g. claude.ai connector install flow)
  issuer: https://api.zillapi.com
  name: oauth2
  sources:
  - well-known/zillapi-oauth-authorization-server.json
  - well-known/zillapi-oauth-protected-resource.json
  type: oauth2
slug: zillapi-authentication
source_filename: zillapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/zillapi-openapi-original.json\ndocs: https://zillapi.com/authentication/\nadditional_sources:\n  - https://zillapi.com/.well-known/oauth-protected-resource\n  - https://zillapi.com/.well-known/oauth-authorization-server\n  - https://zillapi.com/auth.md\nsummary:\n  types:\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\nnotes: >-\n  Zillapi accepts two auth modes against one account and one scope. (1) A long-lived API key sent as\n  `Authorization: Bearer zk_<key>`, issued in the dashboard, used for both the /v1 REST surface and the\n  hosted MCP server. (2) OAuth 2.1 authorization-code + PKCE with RFC 7591 Dynamic Client Registration,\n  for remote-MCP connectors. The OpenAPI only declares the bearer scheme; the OAuth surface is published\n  in the RFC 8414 / RFC 9728 well-known metadata, not in the spec.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n\
  \    bearerFormat: API key (zk_*)\n    sources:\n      - openapi/zillapi-openapi-original.json\n    key_format:\n      prefix: zk_\n      body: 43 characters, URL-safe base64 of 32 random bytes\n      total_length: 46\n    storage: >-\n      Plaintext shown once at creation; provider states it stores only the SHA-256 hash and cannot\n      recover the original.\n    management_url: https://zillapi.com/app/keys/\n    signup_url: https://zillapi.com/signup\n    rotation:\n      documented: true\n      procedure:\n        - Create a new key in the dashboard\n        - Roll it into the environment\n        - Confirm traffic on the new key under Usage\n        - Revoke the old key\n      revocation: immediate — calls on a revoked key return 401 invalid_api_key within seconds\n  - name: oauth2\n    type: oauth2\n    sources:\n      - well-known/zillapi-oauth-authorization-server.json\n      - well-known/zillapi-oauth-protected-resource.json\n    issuer: https://api.zillapi.com\n    flows:\n\
  \      - flow: authorizationCode\n        authorizationUrl: https://api.zillapi.com/oauth/authorize\n        tokenUrl: https://api.zillapi.com/oauth/token\n        revocationUrl: https://api.zillapi.com/oauth/revoke\n        registrationUrl: https://api.zillapi.com/oauth/register\n        pkce: S256\n        pkce_required: true\n        token_endpoint_auth_methods: [none]\n        scopes:\n          mcp:access: Access the Zillapi MCP server and the /v1 REST surface\n    dynamic_client_registration:\n      supported: true\n      standard: RFC 7591\n      endpoint: https://api.zillapi.com/oauth/register\n    intended_for: remote-MCP connectors (e.g. claude.ai connector install flow)\nerrors:\n  - {status: 401, code: missing_api_key, cause: No Authorization header}\n  - {status: 401, code: invalid_api_key, cause: Bad format, unknown key, or revoked}\n  - {status: 403, code: account_suspended, cause: Account is suspended or closed}\n  - {status: 402, code: out_of_credits, cause: Credit balance\
  \ reached 0}\n  - {status: 429, code: rate_limited, cause: Per-minute rate limit hit}\nguidance:\n  - Server-side only; never embed a key in browser or mobile code that ships to users\n  - One key per environment (staging vs production)\n  - One key per service so they can be revoked independently\ncross_links:\n  scopes: scopes/zillapi-scopes.yml\n  conventions: conventions/zillapi-conventions.yml\n  well_known: well-known/zillapi-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/authentication/zillapi-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- real estate
- proptech
- property data
- zillow
- zestimate
- valuation
- AVM
- listings
- MCP
- AI agent
- REST API
---
