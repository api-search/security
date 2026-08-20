---
api_key_in:
- header
api_specs:
- filename: gamesight-measurement-api-openapi.yml
  format: yaml
  label: Gamesight Measurement API
  slug: gamesight-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-measurement-api-openapi.yml
- filename: gamesight-reporting-api-openapi.yml
  format: yaml
  label: Gamesight Reporting API
  slug: gamesight-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-reporting-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Gamesight Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Gamesight secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Gamesight
provider_slug: gamesight
scheme_count: 2
schemes:
- applies_to:
  - openapi/gamesight-measurement-api-openapi.yml
  - openapi/gamesight-reporting-api-openapi.yml
  description: An opaque Gamesight API key passed in the Authorization header on every request. The key's permissions are fixed when it is created in the console. Reporting API keys carry the Reporting, Aggregate Reporting, GDPR, or Audit scope; the Measurement (in-game/web ingest) key is a separate credential provisioned under Management > In-Game Integration.
  docs: https://docs.gamesight.io/docs/api-key-management
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  scopes:
  - Reporting
  - Aggregate Reporting
  - GDPR
  - Audit
  - Event Measurement
  sources:
  - openapi/_original/gamesight-measurement-openapi.json
  - openapi/_original/gamesight-reporting-openapi.json
  type: apiKey
- applies_to:
  - mcp/gamesight-mcp.yml
  description: OAuth 2.0 authorization-code flow with PKCE (S256) and RFC 7591 dynamic client registration, issued by console.gamesight.io. NOT documented in the public developer docs — discovered by probing /.well-known/ on the API hosts. Its single advertised scope, "mcp", gates the hosted MCP server at https://console.gamesight.io/mcp. It does not apply to the two REST APIs, which remain API-key authenticated.
  documented: false
  dynamic_client_registration: https://console.gamesight.io/api/app/oauth/register
  flows:
  - authorizationUrl: https://console.gamesight.io/authorize
    flow: authorizationCode
    scopes:
      mcp: Access to the Gamesight MCP Server
    tokenUrl: https://console.gamesight.io/api/app/oauth/token
  issuer: https://console.gamesight.io
  name: GamesightOAuth2
  pkce: S256
  revocation_endpoint: https://console.gamesight.io/api/app/oauth/revoke
  sources:
  - well-known/gamesight-oauth-authorization-server.json
  - well-known/gamesight-console-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: gamesight-authentication
source_filename: gamesight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  openapi/gamesight-measurement-api-openapi.yml,\n  openapi/gamesight-reporting-api-openapi.yml,\n  https://api.marketing.gamesight.io/.well-known/oauth-authorization-server\ndocs: https://docs.gamesight.io/reference/authorization\nnote: >-\n  Upgraded from derived to searched on 2026-08-13. The OpenAPI specs declare\n  only the apiKey scheme; the docs add the four key permission scopes, and a\n  live probe of the API hosts found an undocumented OAuth 2.0 authorization\n  server that gates the hosted MCP server. All three are recorded.\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      An opaque Gamesight API key passed in the Authorization header on every\n      request. The key's permissions are fixed when it is created in the console.\n\
  \      Reporting API keys carry the Reporting, Aggregate Reporting, GDPR, or Audit\n      scope; the Measurement (in-game/web ingest) key is a separate credential\n      provisioned under Management > In-Game Integration.\n    scopes:\n      - Reporting\n      - Aggregate Reporting\n      - GDPR\n      - Audit\n      - Event Measurement\n    docs: https://docs.gamesight.io/docs/api-key-management\n    applies_to:\n      - openapi/gamesight-measurement-api-openapi.yml\n      - openapi/gamesight-reporting-api-openapi.yml\n    sources:\n      - openapi/_original/gamesight-measurement-openapi.json\n      - openapi/_original/gamesight-reporting-openapi.json\n  - name: GamesightOAuth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization-code flow with PKCE (S256) and RFC 7591 dynamic\n      client registration, issued by console.gamesight.io. NOT documented in the\n      public developer docs — discovered by probing /.well-known/ on the API\n      hosts. Its single advertised\
  \ scope, \"mcp\", gates the hosted MCP server at\n      https://console.gamesight.io/mcp. It does not apply to the two REST APIs,\n      which remain API-key authenticated.\n    issuer: https://console.gamesight.io\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://console.gamesight.io/authorize\n        tokenUrl: https://console.gamesight.io/api/app/oauth/token\n        scopes:\n          mcp: Access to the Gamesight MCP Server\n    pkce: S256\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n    dynamic_client_registration: https://console.gamesight.io/api/app/oauth/register\n    revocation_endpoint: https://console.gamesight.io/api/app/oauth/revoke\n    documented: false\n    applies_to:\n      - mcp/gamesight-mcp.yml\n    sources:\n      - well-known/gamesight-oauth-authorization-server.json\n      - well-known/gamesight-console-oauth-authorization-server.json\nsso:\n  saml: https://docs.gamesight.io/docs/okta-saml-config\n\
  \  scim: https://docs.gamesight.io/docs/okta-scim-config\n  providers:\n    - Okta\n    - Google Workspace\n  note: Console (human) access supports SAML SSO and SCIM 2.0 user provisioning; this is dashboard access, not API auth.\nref:\n  scopes: scopes/gamesight-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/authentication/gamesight-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Gaming
- Marketing
- Analytics
- Attribution
- Measurements
- Advertising
- Creators
- Game Development
---
