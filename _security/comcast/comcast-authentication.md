---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Comcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comcast declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Comcast
provider_slug: comcast
scheme_count: 3
schemes:
- api: comcast:authentication-api
  credential_headers:
  - x-client-id
  - x-client-secret
  dpop_signing_alg_values_supported:
  - ES256
  - RS256
  flow: client_credentials
  grant_types_supported:
  - client_credentials
  - urn:ietf:params:oauth:grant-type:token-exchange
  id: comcast-sat
  issuer: https://sat-prod.codebig2.net
  jwks_uri: https://sat-prod.codebig2.net/v2/sign-keys/available
  label: Comcast SAT (Security Access Token)
  notes: The docs show credentials sent as x-client-id / x-client-secret request headers against https://sat-prod.codebig2.net/oauth/token, while the discovery document advertises the RFC 6749 client_secret_basic / client_secret_post methods against /v2/ws/token.oauth2. Both are recorded because both are published; a client should treat the discovery document as authoritative and the docs example as the partner-onboarding recipe. Tokens are 24 hours and must be refreshed. SAT clients are provisioned with an allowedPartner value, so the token is partner-scoped as well as client-scoped.
  presented_as: 'Authorization: Bearer <access_token>'
  scopes_returned:
  - x1:compass:piws:read
  - x1:compass:piws:write
  subject_types_supported:
  - public
  - pairwise
  token_endpoint: https://sat-prod.codebig2.net/v2/ws/token.oauth2
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  token_endpoint_auth_signing_alg_values_supported:
  - ES256
  - RS256
  token_endpoint_documented_alias: https://sat-prod.codebig2.net/oauth/token
  token_lifetime_seconds: 86400
  token_type: Bearer
  type: oauth2
- api: comcast:open-ingest-api
  base_url: https://compass-mmpwebservice-prod.codebig2.net
  bearer_format: Comcast SAT access token
  depends_on: comcast-sat
  id: comcast-open-ingest
  label: Open Ingest bearer token
  notes: 'The Open Ingest proxy accepts nothing but a SAT bearer token. Probed anonymously 2026-09-05: every path on this host, including every /.well-known/ path, returns HTTP 401. There is no anonymous surface.'
  scheme: bearer
  type: http
- api: comcast:firebolt-sdk
  capabilities:
  - xrn:firebolt:capability:token:platform
  - xrn:firebolt:capability:token:device
  - xrn:firebolt:capability:token:session
  - xrn:firebolt:capability:token:root
  - xrn:firebolt:capability:token:account
  contract: openrpc/comcast-firebolt-core-openrpc.json
  gated_by: Firebolt capability grants (see scopes/comcast-scopes.yml)
  id: firebolt-authentication-module
  label: Firebolt Authentication module (on-device JSON-RPC)
  methods:
  - Authentication.token
  - Authentication.device
  - Authentication.session
  - Authentication.root
  notes: Authentication.token is marked deprecated as of Firebolt 0.9.0 in the contract itself; the replacement is the per-token-type methods. Tokens resolve to {value, expires, type}. This is a device-local capability check, not an HTTP authorization header.
  token_types:
  - platform
  - device
  - session
  - root
  - account
  transport: JSON-RPC 2.0 over the Firebolt transport
  type: platform-token
slug: comcast-authentication
source_filename: comcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# Comcast — authentication profile\n#\n# Two distinct authentication surfaces, and they are not the same system:\n#\n#  1. COMCAST SAT (Security Access Token) — a real OAuth 2.0 authorization\n#     server for server-to-server partner calls. Confirmed by a live\n#     /.well-known/openid-configuration on sat-prod.codebig2.net (saved verbatim\n#     at well-known/comcast-sat-openid-configuration.json) AND by the published\n#     request/response example on the Open Ingest Endpoints docs page.\n#  2. FIREBOLT ON-DEVICE TOKENS — the Authentication module of the Firebolt Core\n#     OpenRPC contract. This is not an HTTP auth scheme at all; it is a JSON-RPC\n#     method an app calls on the device to obtain a platform, device, session or\n#     root token, gated by Firebolt capability grants rather than by scopes.\ngenerated: '2026-09-05'\nmethod: searched\nmethod_note: >-\n  derive-authentication.py reads OpenAPI securitySchemes and returned nothing\n  for this provider (Comcast\
  \ publishes OpenRPC, not OpenAPI). Written by hand\n  from the fetched discovery document and the provider's own docs.\nsource: >-\n  https://sat-prod.codebig2.net/.well-known/openid-configuration (HTTP 200,\n  application/json, fetched 2026-09-05) and\n  https://docs.developer.comcast.com/docs/endpoints (HTTP 200, fetched 2026-09-05)\ndocs:\n  - https://docs.developer.comcast.com/docs/endpoints\n  - https://docs.developer.comcast.com/docs/081-core-authentication\n  - https://docs.developer.comcast.com/docs/170-core-authentication\nprovider: Comcast\nproviderId: comcast\nschemes:\n  - id: comcast-sat\n    api: comcast:authentication-api\n    type: oauth2\n    flow: client_credentials\n    label: Comcast SAT (Security Access Token)\n    issuer: https://sat-prod.codebig2.net\n    token_endpoint: https://sat-prod.codebig2.net/v2/ws/token.oauth2\n    token_endpoint_documented_alias: https://sat-prod.codebig2.net/oauth/token\n    jwks_uri: https://sat-prod.codebig2.net/v2/sign-keys/available\n\
  \    grant_types_supported:\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:token-exchange\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n    token_endpoint_auth_signing_alg_values_supported:\n      - ES256\n      - RS256\n    dpop_signing_alg_values_supported:\n      - ES256\n      - RS256\n    subject_types_supported:\n      - public\n      - pairwise\n    credential_headers:\n      - x-client-id\n      - x-client-secret\n    token_type: Bearer\n    token_lifetime_seconds: 86400\n    presented_as: 'Authorization: Bearer <access_token>'\n    scopes_returned:\n      - x1:compass:piws:read\n      - x1:compass:piws:write\n    notes: >-\n      The docs show credentials sent as x-client-id / x-client-secret request\n      headers against https://sat-prod.codebig2.net/oauth/token, while the\n      discovery document advertises the RFC 6749 client_secret_basic /\n      client_secret_post methods against /v2/ws/token.oauth2.\
  \ Both are recorded\n      because both are published; a client should treat the discovery document\n      as authoritative and the docs example as the partner-onboarding recipe.\n      Tokens are 24 hours and must be refreshed. SAT clients are provisioned\n      with an allowedPartner value, so the token is partner-scoped as well as\n      client-scoped.\n  - id: comcast-open-ingest\n    api: comcast:open-ingest-api\n    type: http\n    scheme: bearer\n    label: Open Ingest bearer token\n    bearer_format: Comcast SAT access token\n    depends_on: comcast-sat\n    base_url: https://compass-mmpwebservice-prod.codebig2.net\n    notes: >-\n      The Open Ingest proxy accepts nothing but a SAT bearer token. Probed\n      anonymously 2026-09-05: every path on this host, including every\n      /.well-known/ path, returns HTTP 401. There is no anonymous surface.\n  - id: firebolt-authentication-module\n    api: comcast:firebolt-sdk\n    type: platform-token\n    label: Firebolt Authentication\
  \ module (on-device JSON-RPC)\n    transport: JSON-RPC 2.0 over the Firebolt transport\n    contract: openrpc/comcast-firebolt-core-openrpc.json\n    methods:\n      - Authentication.token\n      - Authentication.device\n      - Authentication.session\n      - Authentication.root\n    token_types:\n      - platform\n      - device\n      - session\n      - root\n      - account\n    gated_by: Firebolt capability grants (see scopes/comcast-scopes.yml)\n    capabilities:\n      - xrn:firebolt:capability:token:platform\n      - xrn:firebolt:capability:token:device\n      - xrn:firebolt:capability:token:session\n      - xrn:firebolt:capability:token:root\n      - xrn:firebolt:capability:token:account\n    notes: >-\n      Authentication.token is marked deprecated as of Firebolt 0.9.0 in the\n      contract itself; the replacement is the per-token-type methods. Tokens\n      resolve to {value, expires, type}. This is a device-local capability\n      check, not an HTTP authorization header.\n\
  mtls: false\nopenid_connect:\n  discovery_document_served: true\n  url: https://sat-prod.codebig2.net/.well-known/openid-configuration\n  full_oidc: false\n  note: >-\n    The document is served at the OIDC discovery path but describes an OAuth 2.0\n    authorization server: there is no authorization_endpoint, no\n    userinfo_endpoint, no id_token_signing_alg_values_supported and no\n    scopes_supported. Treat it as RFC 8414 authorization-server metadata served\n    at the OIDC path, not as an OpenID Provider.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comcast/refs/heads/main/authentication/comcast-authentication.yml
summary_line: 3 schemes
tags:
- Cable
- Connected Devices
- Entertainment
- Internet
- Media
- Mobile
- Streaming
- Wireless
- Fortune 100
---
