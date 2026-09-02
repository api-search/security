---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Allo Media Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Allo-Media secures its APIs with oauth2, openIdConnect, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Allo-Media
provider_slug: allo-media
scheme_count: 5
schemes:
- detail: scopes/allo-media-scopes.yml
  issuer: https://id.uh.live/realms/uhlive
  jwks_uri: https://id.uh.live/realms/uhlive/protocol/openid-connect/certs
  name: uhlive_keycloak_oidc
  note: The realm behind every API surface. Advertises PKCE (S256 and plain), private_key_jwt, tls_client_auth with mTLS-bound access tokens, DPoP, token introspection and revocation endpoints, and dynamic client registration. None of this is mentioned in the developer documentation.
  openIdConnectUrl: https://id.uh.live/realms/uhlive/.well-known/openid-configuration
  type: openIdConnect
  verified: probed
- flow: clientCredentials
  name: uhlive_oauth2_client_credentials
  request_body:
    client_id: '{provided by your account manager}'
    client_secret: '{provided by your account manager}'
    grant_type: client_credentials
  scopes:
  - activate
  - stream-h2h
  - stream-h2h-v2
  - stream-h2b
  - voip-callapi
  - scribr
  scopes_note: 'No OAuth scopes are documented anywhere in the provider''s public docs — no scope parameter appears in any example. But the realm''s OIDC discovery document advertises a per-product scope model: `activate`, `stream-h2h`, `stream-h2h-v2`, `stream-h2b`, `scribr`, plus `voip-callapi` for a surface with no documentation page at all. Captured in scopes/allo-media-scopes.yml with per-scope confidence, because `scopes_supported` describes what the authorization server can issue, not what any given client is granted.'
  source: https://docs.allo-media.net/activate-api/rest/authentication/
  token_url: https://id.uh.live/realms/uhlive/protocol/openid-connect/token
  type: oauth2
- applies_to: Activate API (REST) — https://activate.uh.live
  format: bearer {access_token}
  header: Authorization
  in: header
  name: activate_api_bearer
  scheme: bearer
  source: https://docs.allo-media.net/activate-api/rest/authentication/
  token_lifetime_note: '"Token lifetime: 60 minutes" per the Activate API authentication page.'
  token_lifetime_seconds: 3600
  type: http
- applies_to: Stream API for humans (WebSocket) — wss://api.uh.live
  format: wss://api.uh.live/socket/websocket?vsn=2.0.0&jwt={access_token}
  in: query
  name: stream_api_jwt_query
  note: The access token is passed as a URL query parameter on the WebSocket handshake rather than an Authorization header. That is normal for browser WebSocket clients (which cannot set headers) but it does mean the token can land in proxy/access logs.
  parameter: jwt
  scheme: bearer
  source: https://docs.allo-media.net/stream-h2h/protocol/
  token_lifetime_note: '"Token validity: 5 minutes" per the Stream API V2 protocol reference — a different, much shorter TTL than the Activate REST token, so an integration holding one token for both surfaces will fail on the stream side first.'
  token_lifetime_seconds: 300
  type: http
- applies_to: JUpload batch audio ingestion (SFTP)
  mechanism: SFTP account credentials
  name: jupload_sftp
  note: 'JUpload is not an HTTP API: audio and metadata are delivered over SFTP, optionally GPG-encrypted with a public key the provider supplies. Recorded here for completeness because it is a credentialed ingestion path, not an OpenAPI securityScheme.'
  optional_payload_encryption: GPG (public key supplied by the provider)
  source: https://docs.allo-media.net/jupload/encryption/
  type: other
slug: allo-media-authentication
source_filename: allo-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://docs.allo-media.net/activate-api/rest/authentication/\ndocs:\n  - https://docs.allo-media.net/activate-api/rest/authentication/\n  - https://docs.allo-media.net/stream-h2h/protocol/\n  - https://docs.allo-media.net/stream-h2h/python/getting-started/\n  - https://docs.allo-media.net/stream-h2b/protocols/authentication/\nnote: >-\n  Derived by reading the provider's own auth documentation, not from an OpenAPI —\n  no machine-readable spec was reachable during this pass (see\n  x-coverage in apis.yml). Every value below is quoted from the docs pages\n  listed above. Credentials themselves are not self-service: the docs state\n  client_id/client_secret \"were provided to you by your account manager\".\nsummary:\n  types: [oauth2, openIdConnect, http]\n  oauth2_flows: [clientCredentials]\n  oauth2_flows_available_but_undocumented:\n    [authorizationCode, deviceCode, password, refreshToken, tokenExchange, jwtBearer, uma,\
  \ ciba]\n  bearer_in: [header, query]\n  identity_provider: Keycloak (realm `uhlive`)\n  oidc_discovery: https://id.uh.live/realms/uhlive/.well-known/openid-configuration\n  oidc_discovery_verified: true\n  scopes_documented: false\n  scopes_discovered: 19\n  self_service_signup: false\nx-discovery-upgrade:\n  date: '2026-08-17'\n  note: >-\n    This profile was upgraded from documentation-only to probe-verified. The\n    provider's docs describe one flow and no scopes; the realm's OIDC discovery\n    document (captured verbatim at\n    well-known/allo-media-openid-configuration.json, HTTP 200,\n    application/json, 6,625 bytes) exposes a full authorization-server\n    configuration including a per-product scope model, mTLS-bound access tokens,\n    DPoP, private_key_jwt and dynamic client registration. Full detail in\n    scopes/allo-media-scopes.yml.\n  discovery_url: https://id.uh.live/realms/uhlive/.well-known/openid-configuration\n  http_status: 200\nschemes:\n  - name: uhlive_keycloak_oidc\n\
  \    type: openIdConnect\n    openIdConnectUrl: https://id.uh.live/realms/uhlive/.well-known/openid-configuration\n    issuer: https://id.uh.live/realms/uhlive\n    jwks_uri: https://id.uh.live/realms/uhlive/protocol/openid-connect/certs\n    verified: probed\n    detail: scopes/allo-media-scopes.yml\n    note: >-\n      The realm behind every API surface. Advertises PKCE (S256 and plain),\n      private_key_jwt, tls_client_auth with mTLS-bound access tokens, DPoP,\n      token introspection and revocation endpoints, and dynamic client\n      registration. None of this is mentioned in the developer documentation.\n  - name: uhlive_oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://id.uh.live/realms/uhlive/protocol/openid-connect/token\n    request_body:\n      client_id: \"{provided by your account manager}\"\n      client_secret: \"{provided by your account manager}\"\n      grant_type: client_credentials\n    scopes: [activate, stream-h2h,\
  \ stream-h2h-v2, stream-h2b, voip-callapi, scribr]\n    scopes_note: >-\n      No OAuth scopes are documented anywhere in the provider's public docs — no\n      scope parameter appears in any example. But the realm's OIDC discovery\n      document advertises a per-product scope model: `activate`, `stream-h2h`,\n      `stream-h2h-v2`, `stream-h2b`, `scribr`, plus `voip-callapi` for a surface\n      with no documentation page at all. Captured in\n      scopes/allo-media-scopes.yml with per-scope confidence, because\n      `scopes_supported` describes what the authorization server can issue, not\n      what any given client is granted.\n    source: https://docs.allo-media.net/activate-api/rest/authentication/\n  - name: activate_api_bearer\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"bearer {access_token}\"\n    token_lifetime_seconds: 3600\n    token_lifetime_note: >-\n      \"Token lifetime: 60 minutes\" per the Activate API authentication\
  \ page.\n    applies_to: Activate API (REST) — https://activate.uh.live\n    source: https://docs.allo-media.net/activate-api/rest/authentication/\n  - name: stream_api_jwt_query\n    type: http\n    scheme: bearer\n    in: query\n    parameter: jwt\n    format: \"wss://api.uh.live/socket/websocket?vsn=2.0.0&jwt={access_token}\"\n    token_lifetime_seconds: 300\n    token_lifetime_note: >-\n      \"Token validity: 5 minutes\" per the Stream API V2 protocol reference — a\n      different, much shorter TTL than the Activate REST token, so an\n      integration holding one token for both surfaces will fail on the stream\n      side first.\n    applies_to: Stream API for humans (WebSocket) — wss://api.uh.live\n    source: https://docs.allo-media.net/stream-h2h/protocol/\n    note: >-\n      The access token is passed as a URL query parameter on the WebSocket\n      handshake rather than an Authorization header. That is normal for browser\n      WebSocket clients (which cannot set headers)\
  \ but it does mean the token\n      can land in proxy/access logs.\n  - name: jupload_sftp\n    type: other\n    mechanism: SFTP account credentials\n    applies_to: JUpload batch audio ingestion (SFTP)\n    optional_payload_encryption: GPG (public key supplied by the provider)\n    source: https://docs.allo-media.net/jupload/encryption/\n    note: >-\n      JUpload is not an HTTP API: audio and metadata are delivered over SFTP,\n      optionally GPG-encrypted with a public key the provider supplies. Recorded\n      here for completeness because it is a credentialed ingestion path, not an\n      OpenAPI securityScheme.\nx-gaps:\n  - No self-service credential issuance; every documented path routes through an\n    account manager, so no anonymous or trial token could be obtained to verify\n    the flows live.\n  - No documented token refresh/rotation guidance beyond the two TTLs.\n  - No documented scopes, audiences, or least-privilege model on the realm.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allo-media/refs/heads/main/authentication/allo-media-authentication.yml
summary_line: oauth2/openIdConnect/http · 5 schemes
tags:
- Company
- Ai Data
- Speech Recognition
- Speech-to-Text
- Conversation Intelligence
- Call Tracking
- Voice AI
- Natural Language Processing
- Call Analytics
- Contact Center
- Speech Analytics
- Transcription
- France
---
