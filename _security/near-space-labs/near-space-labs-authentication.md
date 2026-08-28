---
api_key_in: []
api_specs:
- filename: near-space-labs-tile-service.json
  format: json
  label: Near Space Labs Tile Service
  slug: near-space-labs-tile-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near-space-labs/refs/heads/main/openapi/near-space-labs-tile-service.json
- filename: near-space-labs-oauth-service.json
  format: json
  label: Near Space Labs OAuth Service
  slug: near-space-labs-oauth-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near-space-labs/refs/heads/main/openapi/near-space-labs-oauth-service.json
auth_types: []
description: 'Every Near Space Labs API endpoint is authenticated. There are two credential shapes, both minted from the same NSL client id + client secret pair: a 60-minute OAuth 2.0 client-credentials Bearer JWT, and a one-year static API key passed in the query string. Credentials are issued by Near Space Labs sales/onboarding — there is no self-service signup.'
kind: authentication
layout: security
method: searched
name: Near Space Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Near Space Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Near Space Labs
provider_slug: near-space-labs
scheme_count: 2
schemes:
- docs: https://docs.nearspacelabs.com/authentication
  flow: clientCredentials
  id: oauth2_client_credentials
  presented_as: 'Authorization: Bearer <access_token>'
  refresh: No refresh token is issued. Re-POST /oauth/token. Docs advise refreshing at ~55 minutes (current_time > token_issued_at + expires_in - 300) to keep a 5-minute safety buffer.
  request_fields:
    audience: https://api.nearspacelabs.com (required, constant)
    client_id: Your NSL client id (required)
    client_secret: Your NSL client secret (required)
    grant_type: client_credentials (required)
  request_media_type: application/json
  response_fields:
    access_token: 'JWT to present as `Authorization: Bearer <access_token>`'
    expires_in: 3600 (seconds)
    token_type: Bearer
  scopes: []
  scopes_note: The API publishes no OAuth scope surface. The token request carries no `scope` parameter, the docs document none, and neither Swagger contract declares securityDefinitions. Permissions are attached to the credential pair by Near Space Labs, not selected by the client. `scopes/` is therefore intentionally not emitted for this provider.
  token_endpoint: https://api.nearspacelabs.net/oauth/token
  ttl_seconds: 3600
  type: oauth2
- docs: https://docs.nearspacelabs.com/authentication
  example_usage: https://api.nearspacelabs.net/tile/v2/{surveyid}/{z}/{x}/{y}?api_key=<api_key>
  id: static_api_key
  in: query
  intended_for: Embedding tiles in a web map, sharing a demo, or any client with no token-refresh logic.
  name: api_key
  parity: '"The key carries the same permissions and contract as your OAuth tokens, so it works anywhere a Bearer token does." — docs.nearspacelabs.com/authentication'
  presented_as: ?api_key=<api_key> appended to any authenticated request URL
  provider_warning: 'Quoted verbatim from the docs: "A static key is a bearer credential that lives for a year and travels in the URL, where it can end up in server logs and browser history. Treat it like a password and reissue it if it leaks."'
  request_fields:
    client_id: Your NSL client id (required)
    client_secret: Your NSL client secret (required)
  response_fields:
    api_key: A long-lived signed JWT
    expires_in: 31536000 (seconds — one year)
    token_type: Bearer
  token_endpoint: https://api.nearspacelabs.net/oauth/static_key
  ttl_seconds: 31536000
  type: apiKey
slug: near-space-labs-authentication
source_filename: near-space-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://docs.nearspacelabs.com/authentication and https://docs.nearspacelabs.com/api/oauth,\n  cross-checked against the provider's own Swagger 2.0 contracts at\n  https://api.nearspacelabs.net/oauth/openapi/oauth and https://api.nearspacelabs.net/tile/openapi/tile-server.\ndescription: >-\n  Every Near Space Labs API endpoint is authenticated. There are two credential shapes, both minted\n  from the same NSL client id + client secret pair: a 60-minute OAuth 2.0 client-credentials Bearer\n  JWT, and a one-year static API key passed in the query string. Credentials are issued by Near Space\n  Labs sales/onboarding — there is no self-service signup.\nbase_url: https://api.nearspacelabs.net\nprimary_scheme: oauth2-client-credentials\nschemes:\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://api.nearspacelabs.net/oauth/token\n    request_media_type: application/json\n\
  \    request_fields:\n      client_id: Your NSL client id (required)\n      client_secret: Your NSL client secret (required)\n      audience: 'https://api.nearspacelabs.com (required, constant)'\n      grant_type: client_credentials (required)\n    response_fields:\n      access_token: 'JWT to present as `Authorization: Bearer <access_token>`'\n      expires_in: 3600 (seconds)\n      token_type: Bearer\n    presented_as: 'Authorization: Bearer <access_token>'\n    ttl_seconds: 3600\n    refresh: >-\n      No refresh token is issued. Re-POST /oauth/token. Docs advise refreshing at ~55 minutes\n      (current_time > token_issued_at + expires_in - 300) to keep a 5-minute safety buffer.\n    scopes: []\n    scopes_note: >-\n      The API publishes no OAuth scope surface. The token request carries no `scope` parameter, the\n      docs document none, and neither Swagger contract declares securityDefinitions. Permissions are\n      attached to the credential pair by Near Space Labs, not selected\
  \ by the client. `scopes/` is\n      therefore intentionally not emitted for this provider.\n    docs: https://docs.nearspacelabs.com/authentication\n  - id: static_api_key\n    type: apiKey\n    in: query\n    name: api_key\n    token_endpoint: https://api.nearspacelabs.net/oauth/static_key\n    request_fields:\n      client_id: Your NSL client id (required)\n      client_secret: Your NSL client secret (required)\n    response_fields:\n      api_key: A long-lived signed JWT\n      expires_in: 31536000 (seconds — one year)\n      token_type: Bearer\n    presented_as: '?api_key=<api_key> appended to any authenticated request URL'\n    ttl_seconds: 31536000\n    example_usage: https://api.nearspacelabs.net/tile/v2/{surveyid}/{z}/{x}/{y}?api_key=<api_key>\n    intended_for: >-\n      Embedding tiles in a web map, sharing a demo, or any client with no token-refresh logic.\n    parity: >-\n      \"The key carries the same permissions and contract as your OAuth tokens, so it works anywhere\n\
  \      a Bearer token does.\" — docs.nearspacelabs.com/authentication\n    docs: https://docs.nearspacelabs.com/authentication\n    provider_warning: >-\n      Quoted verbatim from the docs: \"A static key is a bearer credential that lives for a year and\n      travels in the URL, where it can end up in server logs and browser history. Treat it like a\n      password and reissue it if it leaks.\"\ncredential_issuance:\n  self_service: false\n  route: https://www.nearspacelabs.com/contact\n  note: >-\n    NSL_ID / NSL_SECRET are provisioned through sales onboarding. No developer sign-up, no free\n    tier, no key-provisioning endpoint is published.\nfailure_modes:\n  '401': Token missing, expired, or invalid — or an incorrect NSL_ID / NSL_SECRET on /oauth/token.\n  '403': Authenticated but insufficient permissions for the resource.\ndiscovery:\n  openid_configuration: null\n  oauth_authorization_server: null\n  note: >-\n    No /.well-known/openid-configuration and no /.well-known/oauth-authorization-server\
  \ on any host\n    (all 404 — see well-known/near-space-labs-well-known.yml). The token endpoint is discoverable\n    only from prose docs and the OAuth Service Swagger contract.\nspec_gap:\n  observed: >-\n    Neither published Swagger 2.0 document declares `securityDefinitions`, and no operation carries a\n    `security` block, even though the OAuth Service description states \"Authentication is required for\n    all endpoints\" and every tile operation documents 401/403 responses.\n  consequence: >-\n    A code generator or agent reading either contract in isolation would generate an unauthenticated\n    client. Captured as an enhancement in overlays/near-space-labs-tile-service-overlay.yaml and\n    overlays/near-space-labs-oauth-service-overlay.yaml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/near-space-labs/refs/heads/main/authentication/near-space-labs-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Earth Observation
- Aerial Imagery
- Geospatial
- Satellite and Remote Sensing
- Mapping
- Tiles
- Insurance
- Government
- Utilities
- Location
- Imagery
---
