---
api_key_in: []
api_specs:
- filename: ironfang-openapi.yaml
  format: yaml
  label: Renderwolf API
  slug: renderwolf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ironfang Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ironfang secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ironfang
provider_slug: ironfang
scheme_count: 2
schemes:
- description: 'An API key from the portal, sent as `Authorization: Bearer <key>`.'
  failure_codes:
  - code: invalid_api_key
    meaning: missing or unrecognised key
    status: 401
  - code: insufficient_scope
    meaning: key does not carry the scope the operation needs
    status: 403
  key_management:
    created_at: https://portal.ironfang.uk
    revocable: true
    shown_once: true
    storage: hashed - a lost key is replaced, never recovered
  name: apiKey
  scheme: bearer
  scope_note: Key scopes are chosen at creation and cannot be widened afterwards; broader access requires a new key. Keys minted before scopes existed carry no scopes and retain full access for backward compatibility. A call outside the key's scopes returns 403 insufficient_scope naming the missing scope.
  scoped: true
  sources:
  - openapi/ironfang-openapi.yaml
  - https://ironfang.uk/renderwolf/docs#auth
  surface: REST
  type: http
- client_identification:
  - Client ID Metadata Document (CIMD) - an HTTPS URL as the client id; preferred
  - public Dynamic Client Registration with PKCE
  description: OAuth 2.1 authorization-code flow with PKCE (S256) against id.ironfang.uk, used only by MCP clients reaching https://mcp.ironfang.uk/mcp. The access token is audience-bound to the MCP resource; product calls are made with a separate two-minute delegated token minted per call.
  discovery:
    authorization_server: https://id.ironfang.uk/.well-known/oauth-authorization-server
    jwks_uri: https://id.ironfang.uk/oauth/jwks
    openid_configuration: https://id.ironfang.uk/.well-known/openid-configuration
    protected_resource: https://mcp.ironfang.uk/.well-known/oauth-protected-resource
    registration_endpoint: https://id.ironfang.uk/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://id.ironfang.uk/oauth/authorize
      refreshUrl: https://id.ironfang.uk/oauth/token
      tokenUrl: https://id.ironfang.uk/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://id.ironfang.uk
  live_scope_check: A scope is re-checked against the person's organisation permission on every call - losing a permission ends access the same minute.
  name: ironfangOAuth
  pkce: S256
  resource_indicator: resource=https://mcp.ironfang.uk/mcp (RFC 8707)
  sources:
  - well-known/ironfang-oauth-protected-resource.json
  - well-known/ironfang-oauth-authorization-server.json
  - https://ironfang.uk/docs/mcp
  surface: MCP
  tenancy: one connection is one person, one organisation, one client
  token_lifetime: short-lived, rotating refresh token; revocation ends access within 30 seconds
  type: oauth2
slug: ironfang-authentication
source_filename: ironfang-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://ironfang.uk/renderwolf/docs#auth\ndocs: https://ironfang.uk/renderwolf/docs#auth\nderived_from: openapi/ironfang-openapi.yaml\nsummary:\n  types:\n    - http\n    - oauth2\n  note: >-\n    Two distinct credentials serve two distinct surfaces. The REST API takes a long-lived\n    bearer API key minted in the portal. The MCP server refuses API keys outright and takes\n    only a short-lived OAuth 2.1 access token from id.ironfang.uk. Ironfang states each\n    surface rejects the other's token.\nschemes:\n  - name: apiKey\n    type: http\n    scheme: bearer\n    surface: REST\n    description: 'An API key from the portal, sent as `Authorization: Bearer <key>`.'\n    key_management:\n      created_at: https://portal.ironfang.uk\n      shown_once: true\n      storage: hashed - a lost key is replaced, never recovered\n      revocable: true\n    scoped: true\n    scope_note: >-\n      Key scopes are chosen at creation and\
  \ cannot be widened afterwards; broader access\n      requires a new key. Keys minted before scopes existed carry no scopes and retain full\n      access for backward compatibility. A call outside the key's scopes returns\n      403 insufficient_scope naming the missing scope.\n    failure_codes:\n      - status: 401\n        code: invalid_api_key\n        meaning: missing or unrecognised key\n      - status: 403\n        code: insufficient_scope\n        meaning: key does not carry the scope the operation needs\n    sources:\n      - openapi/ironfang-openapi.yaml\n      - https://ironfang.uk/renderwolf/docs#auth\n  - name: ironfangOAuth\n    type: oauth2\n    surface: MCP\n    description: >-\n      OAuth 2.1 authorization-code flow with PKCE (S256) against id.ironfang.uk, used only by\n      MCP clients reaching https://mcp.ironfang.uk/mcp. The access token is audience-bound to\n      the MCP resource; product calls are made with a separate two-minute delegated token\n      minted per\
  \ call.\n    issuer: https://id.ironfang.uk\n    flows:\n      authorizationCode:\n        authorizationUrl: https://id.ironfang.uk/oauth/authorize\n        tokenUrl: https://id.ironfang.uk/oauth/token\n        refreshUrl: https://id.ironfang.uk/oauth/token\n    discovery:\n      protected_resource: https://mcp.ironfang.uk/.well-known/oauth-protected-resource\n      authorization_server: https://id.ironfang.uk/.well-known/oauth-authorization-server\n      openid_configuration: https://id.ironfang.uk/.well-known/openid-configuration\n      jwks_uri: https://id.ironfang.uk/oauth/jwks\n      registration_endpoint: https://id.ironfang.uk/oauth/register\n    client_identification:\n      - Client ID Metadata Document (CIMD) - an HTTPS URL as the client id; preferred\n      - public Dynamic Client Registration with PKCE\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n      - 'urn:ietf:params:oauth:grant-type:token-exchange'\n    pkce: S256\n\
  \    resource_indicator: 'resource=https://mcp.ironfang.uk/mcp (RFC 8707)'\n    token_lifetime: short-lived, rotating refresh token; revocation ends access within 30 seconds\n    tenancy: one connection is one person, one organisation, one client\n    live_scope_check: >-\n      A scope is re-checked against the person's organisation permission on every call - losing\n      a permission ends access the same minute.\n    sources:\n      - well-known/ironfang-oauth-protected-resource.json\n      - well-known/ironfang-oauth-authorization-server.json\n      - https://ironfang.uk/docs/mcp\nsigned_urls:\n  description: >-\n    A third, credential-free access path. POST /v1/sign mints a GET URL whose HMAC signature\n    covers every parameter and the metering account, so it can be embedded in an <img> or\n    og:image tag without exposing the API key.\n  operations:\n    - createSignedUrl\n    - renderSignedUrl\n  ttl: ttl_hours, 0 = never expires (REST); MCP refuses permanent links and caps\
  \ at 24 hours\n  failure_code: 403 bad_signature\nx-findings:\n  - id: key-prefix-disagreement\n    detail: >-\n      The published OpenAPI's info.description documents the key prefix as `rw_live_...`, while\n      the API reference at ironfang.uk/renderwolf/docs and the renderwolf-cli README both\n      document `if_live_...`. Recorded, not resolved - a consumer reading only the contract gets\n      the wrong prefix.\n    evidence:\n      - https://api.ironfang.uk/openapi.yaml\n      - https://ironfang.uk/renderwolf/docs\n      - https://raw.githubusercontent.com/ironfang-ltd/renderwolf-cli/main/README.md\n  - id: oauth-absent-from-contract\n    detail: >-\n      The OpenAPI declares only the apiKey bearer scheme. The OAuth 2.1 model that governs the\n      MCP surface is documented in prose and in the two well-known documents, but appears in no\n      machine-readable contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/authentication/ironfang-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Developer Tools
- Screenshot API
- Website Screenshot
- HTML-to-PDF
- PDF API
- Image API
- OG Image API
- QR Code API
- Website-to-Video
- Rendering Infrastructure
- MCP
- UK-hosted
---
