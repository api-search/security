---
api_key_in: []
api_specs:
- filename: rockbot-audio-messaging-api-openapi.yml
  format: yaml
  label: Rockbot Audio Messaging API
  slug: rockbot-audio-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-audio-messaging-api-openapi.yml
- filename: rockbot-auth-api-openapi.yml
  format: yaml
  label: Rockbot Auth API
  slug: rockbot-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-auth-api-openapi.yml
- filename: rockbot-data-api-openapi.yml
  format: yaml
  label: Rockbot Data API
  slug: rockbot-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-data-api-openapi.yml
- filename: rockbot-devices-api-openapi.yml
  format: yaml
  label: Rockbot Devices API
  slug: rockbot-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-devices-api-openapi.yml
- filename: rockbot-music-api-openapi.yml
  format: yaml
  label: Rockbot Music API
  slug: rockbot-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-music-api-openapi.yml
- filename: rockbot-signage-api-openapi.yml
  format: yaml
  label: Rockbot Signage API
  slug: rockbot-signage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-signage-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Rockbot Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- deviceCode
overview: Rockbot secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and deviceCode flow(s).
provider_name: Rockbot
provider_slug: rockbot
scheme_count: 2
schemes:
- applies_to: https://api.rockbot.com/v5
  description: 'OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET (issued by Rockbot support) at the token endpoint for a 24-hour bearer ACCESS_TOKEN, then send it as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.rockbot.com/v5/api-clients/token
  header: 'Authorization: Bearer ACCESS_TOKEN'
  name: oauth2
  onboarding: Email support@rockbot.com with subject "Rockbot API Access Request", a link to your Dashboard, and the features you want. The email must come from the address tied to your Rockbot user. On approval you receive a CLIENT_ID and a ONE-TIME link to retrieve the CLIENT_SECRET at /v5/api-clients/CLIENT_ID/secret?one_time_code=... — the secret is shown once and never again.
  request_format: 'POST application/json with {"client_id": "...", "client_secret": "..."} — NOT the RFC 6749 form-encoded grant_type=client_credentials body. A standards-compliant OAuth client library will not work unmodified.'
  scope_model: '"Your credentials only grant access to the scopes you requested." Scopes exist and are bound to the client at issuance, but Rockbot publishes no scope reference — see scopes/rockbot-scopes.yml.'
  sources:
  - https://developer.rockbot.com/start.html
  - openapi/rockbot-auth-api-openapi.yml
  surface: REST v5 API
  token_ttl_hours: 24
  token_type: bearer
  type: oauth2
- applies_to: https://api.rockbot.com/v5/mcp
  authorization_endpoint: https://auth.rockbot.com/application/o/authorize/
  bearer_methods_supported:
  - header
  challenge: 'An unauthenticated call returns HTTP 401 with body `no bearer token` and WWW-Authenticate: Bearer resource_metadata="https://api.rockbot.com/.well-known/oauth-protected-resource/v5/mcp"'
  code_challenge_methods_supported:
  - S256
  - plain
  description: OpenID Connect / OAuth 2.0 against Rockbot's self-hosted authentik. Used only by the MCP surface. Advertises standard OIDC scopes; no Rockbot resource scopes appear in discovery.
  device_authorization_endpoint: https://auth.rockbot.com/application/o/device/
  discovery:
    openid_configuration: https://auth.rockbot.com/application/o/mcp-server/.well-known/openid-configuration
    protected_resource_metadata: https://api.rockbot.com/.well-known/oauth-protected-resource/v5/mcp
    protected_resource_metadata_spec: RFC 9728
    saved: well-known/rockbot-mcp-authorization-server.json
  grant_types_supported:
  - authorization_code
  - refresh_token
  - implicit
  - client_credentials
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://auth.rockbot.com/application/o/introspect/
  issuer: https://auth.rockbot.com/application/o/mcp-server/
  jwks_uri: https://auth.rockbot.com/application/o/mcp-server/jwks/
  name: mcp-oauth
  onboarding: Not documented. No public client registration endpoint is advertised (registration_endpoint is absent from the discovery document), and dynamic client registration was not offered, so obtaining MCP credentials appears to require Rockbot to provision them.
  revocation_endpoint: https://auth.rockbot.com/application/o/revoke/
  scopes_supported:
  - openid
  - email
  - profile
  software: authentik 2026.5.4
  sources:
  - https://api.rockbot.com/.well-known/oauth-protected-resource
  - https://auth.rockbot.com/application/o/mcp-server/.well-known/openid-configuration
  - mcp/rockbot-mcp.yml
  surface: Rockbot MCP server
  token_endpoint: https://auth.rockbot.com/application/o/token/
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
  userinfo_endpoint: https://auth.rockbot.com/application/o/userinfo/
slug: rockbot-authentication
source_filename: rockbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developer.rockbot.com/start.html +\n  https://api.rockbot.com/.well-known/oauth-protected-resource +\n  https://auth.rockbot.com/application/o/mcp-server/.well-known/openid-configuration\nnotes: >-\n  UPGRADED from derived to searched. Rockbot runs TWO SEPARATE AUTHENTICATION\n  SURFACES with different issuers, different grants, and different onboarding —\n  a fact visible nowhere in the developer documentation, and the single most\n  important thing an integrator needs to know here. Surface 1 is the documented\n  v5 REST API (OAuth 2.0 client-credentials against api.rockbot.com, credentials\n  issued by a human at Rockbot support). Surface 2 is the undocumented Rockbot\n  MCP server (OAuth against a self-hosted authentik identity provider at\n  auth.rockbot.com). A token minted for one will not authenticate the other.\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  oauth2_flows:\n    - clientCredentials\n\
  \    - authorizationCode\n    - deviceCode\n  surfaces: 2\nschemes:\n  - name: oauth2\n    type: oauth2\n    surface: REST v5 API\n    applies_to: https://api.rockbot.com/v5\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.rockbot.com/v5/api-clients/token\n        scopes: 0\n    token_type: bearer\n    header: 'Authorization: Bearer ACCESS_TOKEN'\n    token_ttl_hours: 24\n    request_format: >-\n      POST application/json with {\"client_id\": \"...\", \"client_secret\": \"...\"} —\n      NOT the RFC 6749 form-encoded grant_type=client_credentials body. A\n      standards-compliant OAuth client library will not work unmodified.\n    onboarding: >-\n      Email support@rockbot.com with subject \"Rockbot API Access Request\", a link\n      to your Dashboard, and the features you want. The email must come from the\n      address tied to your Rockbot user. On approval you receive a CLIENT_ID and\n      a ONE-TIME link to retrieve the CLIENT_SECRET at\n      /v5/api-clients/CLIENT_ID/secret?one_time_code=...\
  \ — the secret is shown\n      once and never again.\n    scope_model: >-\n      \"Your credentials only grant access to the scopes you requested.\" Scopes\n      exist and are bound to the client at issuance, but Rockbot publishes no\n      scope reference — see scopes/rockbot-scopes.yml.\n    description: >-\n      OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET\n      (issued by Rockbot support) at the token endpoint for a 24-hour bearer\n      ACCESS_TOKEN, then send it as `Authorization: Bearer ACCESS_TOKEN`.\n    sources:\n      - https://developer.rockbot.com/start.html\n      - openapi/rockbot-auth-api-openapi.yml\n  - name: mcp-oauth\n    type: openIdConnect\n    surface: Rockbot MCP server\n    applies_to: https://api.rockbot.com/v5/mcp\n    discovery:\n      protected_resource_metadata: https://api.rockbot.com/.well-known/oauth-protected-resource/v5/mcp\n      protected_resource_metadata_spec: RFC 9728\n      openid_configuration: https://auth.rockbot.com/application/o/mcp-server/.well-known/openid-configuration\n\
  \      saved: well-known/rockbot-mcp-authorization-server.json\n    issuer: https://auth.rockbot.com/application/o/mcp-server/\n    software: authentik 2026.5.4\n    authorization_endpoint: https://auth.rockbot.com/application/o/authorize/\n    token_endpoint: https://auth.rockbot.com/application/o/token/\n    userinfo_endpoint: https://auth.rockbot.com/application/o/userinfo/\n    introspection_endpoint: https://auth.rockbot.com/application/o/introspect/\n    revocation_endpoint: https://auth.rockbot.com/application/o/revoke/\n    device_authorization_endpoint: https://auth.rockbot.com/application/o/device/\n    jwks_uri: https://auth.rockbot.com/application/o/mcp-server/jwks/\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - implicit\n      - client_credentials\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n    code_challenge_methods_supported:\
  \ [S256, plain]\n    id_token_signing_alg_values_supported: [RS256]\n    scopes_supported: [openid, email, profile]\n    bearer_methods_supported: [header]\n    challenge: >-\n      An unauthenticated call returns HTTP 401 with body `no bearer token` and\n      WWW-Authenticate: Bearer\n      resource_metadata=\"https://api.rockbot.com/.well-known/oauth-protected-resource/v5/mcp\"\n    onboarding: >-\n      Not documented. No public client registration endpoint is advertised\n      (registration_endpoint is absent from the discovery document), and dynamic\n      client registration was not offered, so obtaining MCP credentials appears\n      to require Rockbot to provision them.\n    description: >-\n      OpenID Connect / OAuth 2.0 against Rockbot's self-hosted authentik. Used\n      only by the MCP surface. Advertises standard OIDC scopes; no Rockbot\n      resource scopes appear in discovery.\n    sources:\n      - https://api.rockbot.com/.well-known/oauth-protected-resource\n     \
  \ - https://auth.rockbot.com/application/o/mcp-server/.well-known/openid-configuration\n      - mcp/rockbot-mcp.yml\nobservations:\n  - >-\n    PKCE is supported (S256), but `plain` is also advertised, and the implicit\n    and password grants remain enabled on the authentik provider. Those are\n    deprecated grants and are worth flagging to Rockbot.\n  - >-\n    Invalid client credentials at the REST token endpoint return HTTP 500, not\n    401/400 — see errors/rockbot-problem-types.yml. Clients must not treat that\n    500 as retryable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/authentication/rockbot-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Music
- Digital Signage
- Audio Messaging
- Retail Media
- In-Location Media
- Media
- Entertainment
---
