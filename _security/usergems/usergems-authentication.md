---
api_key_in:
- header
api_specs:
- filename: usergems-accounts-api-openapi.yml
  format: yaml
  label: UserGems Accounts API
  slug: usergems-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-accounts-api-openapi.yml
- filename: usergems-contacts-api-openapi.yml
  format: yaml
  label: UserGems Contacts API
  slug: usergems-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-contacts-api-openapi.yml
- filename: usergems-privacy-api-openapi.yml
  format: yaml
  label: UserGems Privacy API
  slug: usergems-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-privacy-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: UserGems runs two independent authentication models on two different hosts. The REST ingestion API (api.usergems.com/v1) uses a single company-wide API key in an X-Api-Key header. The MCP server (app.usergems.com/mcp/usergems) uses OAuth 2.0 authorization-code + PKCE with dynamic client registration and a single scope, delegating each caller the permissions of their own UserGems login. They do not share credentials.
kind: authentication
layout: security
method: searched
name: Usergems Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: UserGems secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: UserGems
provider_slug: usergems
scheme_count: 2
schemes:
- blast_radius: 'Provider-stated: "The API is write-only, so a leaked key cannot expose any of your data. The risk is that an unauthorized party could write incorrect data to your account."'
  description: 'Customer-issued API key. Request a key from support@usergems.com. The

    key must be included on every request in the X-Api-Key header.'
  granularity: One key per company, shared across all integrations. No per-system keys, no way to isolate a misbehaving integration, and no separate test key.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  provisioning: 'Self-service retrieval, not self-service issuance: "Go to Settings → Connected Applications and scroll to the bottom to find your API Token."'
  rotation: Manual only — "Keys are not auto-rotated — contact your CSM to request a new key if needed."
  sources:
  - openapi/usergems-contacts-api-openapi.yml
  - openapi/usergems-accounts-api-openapi.yml
  - openapi/usergems-privacy-api-openapi.yml
  surface: REST (https://api.usergems.com/v1)
  type: apiKey
- challenge: 'An unauthenticated call returns 401 with WWW-Authenticate: Bearer realm="mcp", resource_metadata="…/.well-known/ oauth-protected-resource/mcp/usergems" (RFC 9728).'
  dynamic_client_registration: https://app.usergems.com/mcp/oauth/register
  flows:
  - authorizationUrl: https://app.usergems.com/mcp/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    refresh_token: true
    scopes:
    - mcp:use
    tokenUrl: https://app.usergems.com/mcp/oauth/token
  identity_binding: Authorization runs against the caller's active UserGems browser session; the consent screen names the signed-in email, and each user carries their own permissions.
  issuer: https://app.usergems.com
  name: UserGemsMCP
  sources:
  - well-known/usergems-oauth-authorization-server.json
  - well-known/usergems-oauth-protected-resource.json
  surface: MCP (https://app.usergems.com/mcp/usergems)
  type: oauth2
slug: usergems-authentication
source_filename: usergems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/usergems-api-openapi.yml\ndocs:\n  - https://app.usergems.com/api/documentation\n  - https://help.usergems.com/article/using-the-usergems-api\n  - https://app.usergems.com/.well-known/oauth-authorization-server\ndescription: >-\n  UserGems runs two independent authentication models on two different hosts.\n  The REST ingestion API (api.usergems.com/v1) uses a single company-wide API key\n  in an X-Api-Key header. The MCP server (app.usergems.com/mcp/usergems) uses\n  OAuth 2.0 authorization-code + PKCE with dynamic client registration and a\n  single scope, delegating each caller the permissions of their own UserGems\n  login. They do not share credentials.\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-Api-Key\n    surface: REST (https://api.usergems.com/v1)\n \
  \   description: |-\n      Customer-issued API key. Request a key from support@usergems.com. The\n      key must be included on every request in the X-Api-Key header.\n    sources:\n      - openapi/usergems-contacts-api-openapi.yml\n      - openapi/usergems-accounts-api-openapi.yml\n      - openapi/usergems-privacy-api-openapi.yml\n    provisioning: >-\n      Self-service retrieval, not self-service issuance: \"Go to Settings →\n      Connected Applications and scroll to the bottom to find your API Token.\"\n    rotation: >-\n      Manual only — \"Keys are not auto-rotated — contact your CSM to request a\n      new key if needed.\"\n    granularity: >-\n      One key per company, shared across all integrations. No per-system keys,\n      no way to isolate a misbehaving integration, and no separate test key.\n    blast_radius: >-\n      Provider-stated: \"The API is write-only, so a leaked key cannot expose any\n      of your data. The risk is that an unauthorized party could write incorrect\n\
  \      data to your account.\"\n  - name: UserGemsMCP\n    type: oauth2\n    surface: MCP (https://app.usergems.com/mcp/usergems)\n    sources:\n      - well-known/usergems-oauth-authorization-server.json\n      - well-known/usergems-oauth-protected-resource.json\n    issuer: https://app.usergems.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.usergems.com/mcp/oauth/authorize\n        tokenUrl: https://app.usergems.com/mcp/oauth/token\n        scopes: [mcp:use]\n        pkce: [S256]\n        refresh_token: true\n    dynamic_client_registration: https://app.usergems.com/mcp/oauth/register\n    challenge: >-\n      An unauthenticated call returns 401 with\n      WWW-Authenticate: Bearer realm=\"mcp\", resource_metadata=\"…/.well-known/\n      oauth-protected-resource/mcp/usergems\" (RFC 9728).\n    identity_binding: >-\n      Authorization runs against the caller's active UserGems browser session;\n      the consent screen names the signed-in email,\
  \ and each user carries their\n      own permissions.\ntransport_security:\n  tls: TLSv1.3 on www, app and api hosts\n  hsts:\n    www.usergems.com: true\n    app.usergems.com: true\n    api.usergems.com: false\n  note: >-\n    Provider statement: \"All data transmitted between UserGems and UserGems users\n    is protected using Transport Layer Security (TLS) and HTTP Strict Transport\n    Security (HSTS).\" Our probe records no HSTS header on api.usergems.com — see\n    security/usergems-domain-security.yml.\ngaps:\n  - No OIDC discovery document (/.well-known/openid-configuration 404s on every host).\n  - No mTLS, no signed requests, no HMAC option on the REST API.\n  - No API-key scoping and no key-level rate isolation.\n  - No sandbox/test credential of any kind.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/authentication/usergems-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Sales Intelligence
- Outbound
- Account Based Marketing
- Champion Tracking
- Job Changes
- Buying Signals
- AI Scoring
- Sales Engagement
- CRM
- Revenue Operations
- Go-To-Market
- MCP
- AI Agents
---
