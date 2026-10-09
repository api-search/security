---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ploid-account-api-openapi.yml
  format: yaml
  label: Ploid Account API
  slug: ploid-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-account-api-openapi.yml
- filename: ploid-discovery-api-openapi.yml
  format: yaml
  label: Ploid Discovery API
  slug: ploid-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-discovery-api-openapi.yml
- filename: ploid-enrichment-api-openapi.yml
  format: yaml
  label: Ploid Enrichment API
  slug: ploid-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-enrichment-api-openapi.yml
- filename: ploid-harness-api-openapi.yml
  format: yaml
  label: Ploid Harness API
  slug: ploid-harness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-harness-api-openapi.yml
- filename: ploid-monitors-api-openapi.yml
  format: yaml
  label: Ploid Monitors API
  slug: ploid-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-monitors-api-openapi.yml
- filename: ploid-people-api-openapi.yml
  format: yaml
  label: Ploid People API
  slug: ploid-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-people-api-openapi.yml
- filename: ploid-search-api-openapi.yml
  format: yaml
  label: Ploid Search API
  slug: ploid-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-search-api-openapi.yml
- filename: ploid-social-api-openapi.yml
  format: yaml
  label: Ploid Social API
  slug: ploid-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-social-api-openapi.yml
- filename: ploid-linked-in-api-openapi.yml
  format: yaml
  label: Ploid Linked In API
  slug: ploid-linked-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-linked-in-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Ploid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ploid secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ploid
provider_slug: ploid
scheme_count: 4
schemes:
- format: Bearer $PLOID_API_KEY
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ploid-openapi.yml
  - https://ploid.com/documentation/getting-started/authentication
  type: http
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/ploid-openapi.yml
  - https://ploid.com/documentation/getting-started/authentication
  type: apiKey
- applies_to: https://api.ploid.com/mcp
  dynamic_client_registration: https://api.ploid.com/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://ploid.com/auth/mcp
      refreshUrl: https://api.ploid.com/oauth/token
      scopes:
        account:read: Read usage and credits or revoke the caller key
        agent:chat: Use the harness context and chat completions
        people:enrich: Enrich supported profile and contact fields
        people:search: Search the public people index
      tokenUrl: https://api.ploid.com/oauth/token
  name: mcpOAuth
  pkce: S256
  revocation: https://api.ploid.com/oauth/revoke
  sources:
  - https://api.ploid.com/.well-known/oauth-authorization-server
  - https://api.ploid.com/.well-known/oauth-protected-resource
  - https://ploid.com/documentation/mcp
  type: oauth2
- applies_to: ploid login and npx @ploid/mcp login (stores a narrowly scoped API key locally)
  flows:
    deviceCode:
      deviceAuthorizationUrl: https://auth.ploid.com/oauth2/device_authorization
      tokenUrl: https://auth.ploid.com/oauth2/token
  issuer: https://auth.ploid.com
  name: deviceAuthorization
  sources:
  - https://auth.ploid.com/.well-known/openid-configuration
  - https://ploid.com/documentation/getting-started/authentication
  type: oauth2
slug: ploid-authentication
source_filename: ploid-authentication.yml
source_heading: Authentication Profile
source_url: openapi/ploid-openapi.yml
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: openapi/ploid-openapi.yml\ndocs: https://ploid.com/documentation/getting-started/authentication\nsources:\n  - openapi/ploid-openapi.yml\n  - https://ploid.com/documentation/getting-started/authentication\n  - https://ploid.com/documentation/mcp\n  - https://api.ploid.com/.well-known/oauth-authorization-server\n  - https://api.ploid.com/.well-known/oauth-protected-resource\n  - https://auth.ploid.com/.well-known/openid-configuration\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  note: >-\n    API requests authenticate with a Ploid API key sent either as Authorization: Bearer $PLOID_API_KEY or\n    as x-api-key: $PLOID_API_KEY; the organization and user identity are derived from the credential. Keys\n    are scoped (see scopes/), shown once (hashed storage), and can be revoked with DELETE /v1/account/key.\n    The hosted MCP server uses OAuth 2.1 (discovery, dynamic client registration,\
  \ authorization code with\n    S256 PKCE, one-hour access tokens, rotating refresh tokens, revocation). The CLI and local MCP package\n    obtain a scoped key through a device authorization flow against auth.ploid.com.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Bearer $PLOID_API_KEY'\n    sources:\n      - openapi/ploid-openapi.yml\n      - https://ploid.com/documentation/getting-started/authentication\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    sources:\n      - openapi/ploid-openapi.yml\n      - https://ploid.com/documentation/getting-started/authentication\n  - name: mcpOAuth\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://ploid.com/auth/mcp\n        tokenUrl: https://api.ploid.com/oauth/token\n        refreshUrl: https://api.ploid.com/oauth/token\n        scopes:\n          agent:chat: Use the harness context and chat completions\n\
  \          people:enrich: Enrich supported profile and contact fields\n          people:search: Search the public people index\n          account:read: Read usage and credits or revoke the caller key\n    pkce: S256\n    dynamic_client_registration: https://api.ploid.com/oauth/register\n    revocation: https://api.ploid.com/oauth/revoke\n    applies_to: https://api.ploid.com/mcp\n    sources:\n      - https://api.ploid.com/.well-known/oauth-authorization-server\n      - https://api.ploid.com/.well-known/oauth-protected-resource\n      - https://ploid.com/documentation/mcp\n  - name: deviceAuthorization\n    type: oauth2\n    flows:\n      deviceCode:\n        deviceAuthorizationUrl: https://auth.ploid.com/oauth2/device_authorization\n        tokenUrl: https://auth.ploid.com/oauth2/token\n    applies_to: 'ploid login and npx @ploid/mcp login (stores a narrowly scoped API key locally)'\n    issuer: https://auth.ploid.com\n    sources:\n      - https://auth.ploid.com/.well-known/openid-configuration\n\
  \      - https://ploid.com/documentation/getting-started/authentication\nkey_hygiene:\n  - Create a separate key for each environment or integration.\n  - Give it only the scopes the integration needs.\n  - Configure daily or monthly budgets where available.\n  - Never expose an API key in browser JavaScript. Send requests through your own server.\n  - Secrets are shown once; a lost secret must be revoked and replaced.\nerrors:\n  - code: missing_api_key\n  - code: invalid_api_key\n  - code: expired_api_key\n  - code: revoked_api_key\n  - code: insufficient_scope\n    status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/authentication/ploid-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- People Data
- People Search
- Contact Enrichment
- Sales Intelligence
- Recruiting
- LinkedIn
- MCP
- Agents
- Data Enrichment
---
