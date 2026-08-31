---
api_key_in: []
api_specs:
- filename: snap-conversion-api-openapi.yml
  format: yaml
  label: Snap Conversion API
  slug: snap-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/openapi/snap-conversion-api-openapi.yml
- filename: snap-events-api-openapi.yml
  format: yaml
  label: Snap Events API
  slug: snap-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/openapi/snap-events-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Snap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snap declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Snap
provider_slug: snap
scheme_count: 0
schemes: []
slug: snap-authentication
source_filename: snap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.snap.com/api/marketing-api/Ads-API/authentication\ndocs:\n  - https://developers.snap.com/api/marketing-api/Ads-API/authentication\n  - https://developers.snap.com/marketing-api/Conversions-API/GetStarted\n  - https://developers.snap.com/marketing-api/Ads-MCP/Introduction\n  - https://developers.snap.com/snap-kit/login-kit/overview\napi: Snap\nsummary: >-\n  Snap runs four distinct authentication models across its developer surface,\n  and they do not share credentials: OAuth 2.0 authorization-code for the\n  Marketing API, a static non-expiring token for the Conversions API, a separate\n  pre-registered-client OAuth flow for the Ads MCP server, and OAuth 2.0 /\n  OpenID Connect for Login Kit.\n\nsummary_types:\n  types: [oauth2, http-bearer, apiKey]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode]\n\nsecurity_schemes:\n  - name: oauth2\n    label: Marketing API OAuth\n    type: oauth2\n    flow:\
  \ authorizationCode\n    authorization_endpoint: https://accounts.snapchat.com/login/oauth2/authorize\n    token_endpoint: https://accounts.snapchat.com/login/oauth2/access_token\n    refresh: true\n    token_type: Bearer\n    access_token_ttl_seconds: 3600\n    header: \"Authorization: Bearer {access_token}\"\n    grants: [authorization_code, refresh_token]\n    parameters:\n      authorize: [client_id, redirect_uri, response_type=code, scope, state]\n      token: [client_id, client_secret, code, grant_type, redirect_uri]\n    scopes:\n      - snapchat-marketing-api\n      - snapchat-offline-conversions-api\n      - snapchat-profile-api\n    discovery:\n      rfc8414: false\n      note: >-\n        accounts.snapchat.com serves no /.well-known/oauth-authorization-server\n        (404, probed 2026-08-13). Endpoints are documented in prose only.\n    ref: scopes/snap-scopes.yml\n\n  - name: mcp-oauth\n    label: Snapchat Ads MCP OAuth\n    type: oauth2\n    flow: authorizationCode\n    issuer:\
  \ https://mcp.snapchat.com/ads\n    resource: https://mcp.snapchat.com/ads\n    authorization_endpoint: https://mcp.snapchat.com/authorize\n    token_endpoint: https://mcp.snapchat.com/token\n    grants: [authorization_code, refresh_token]\n    pkce: S256\n    token_endpoint_auth_methods_supported: [none]\n    dynamic_client_registration: false\n    openid_connect: false\n    scopes: [snapads.read]\n    client_ids_preregistered:\n      - {agent: Claude, client_id: claude-snap-ads}\n      - {agent: Codex, client_id: codex-snap-ads}\n      - {agent: ChatGPT, client_id: chatgpt-snap-ads}\n      - {agent: Antigravity, client_id: antigravity-snap-ads}\n      - {agent: Gemini, client_id: gemini-snap-ads}\n    discovery:\n      rfc8414: true\n      rfc9728: true\n      authorization_server_metadata: well-known/snap-oauth-authorization-server.json\n      protected_resource_metadata: well-known/snap-oauth-protected-resource.json\n      challenge: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.snapchat.com/.well-known/oauth-protected-resource/ads\"\
  '\n    consent_model: >-\n      Two-stage: an Organization/Business Admin approves the agent for the\n      organization, then each member authorizes their own access. Per agent, per\n      member. A member reaches only what their existing Snapchat Ads permissions\n      already allow.\n    revocation: https://accounts.snapchat.com/v2/manage-apps\n    ref: mcp/snap-mcp.yml\n\n  - name: capi-static-token\n    label: Conversions API long-lived token\n    type: apiKey\n    in: query\n    parameter_name: access_token\n    expiry: none\n    rotation: \"Tokens can be generated and deleted from Ads Manager -> Business Details -> Conversions API Tokens.\"\n    required_role: Organization Admin\n    scoping: >-\n      A token may only send events for the Pixel IDs and Snap App IDs that\n      belong to the Org where the token was generated; cross-org use fails.\n    declared_in: openapi/snap-conversions-api-v3-openapi.yml\n    risk_note: >-\n      The V3 spec carries the credential as a QUERY parameter\
  \ on every operation\n      and declares no components.securitySchemes at all. A non-expiring bearer\n      credential in a URL lands in proxy logs, referrer headers and access logs.\n    source: https://developers.snap.com/marketing-api/Conversions-API/GetStarted\n\n  - name: bearerAuth\n    label: Conversions API v2 bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    declared_in: openapi/snap-conversions-api-openapi.yml\n    applied: \"Global security requirement on the v2 spec.\"\n\nsnap_kit_login:\n  summary: >-\n    Snap Kit / Login Kit provides \"Login with Snapchat\" built on OAuth 2.0 with\n    OpenID Connect support for identity, returning approved profile fields.\n  docs: https://developers.snap.com/snap-kit/login-kit/overview\n  type: [oauth2, openIdConnect]\n  sdk_status: >-\n    The Login Kit SDKs that wrapped the OAuth2 service (and supplied a drop-in\n    login button) are being deprecated. Snap's guidance is to implement OAuth2\n    directly; the underlying\
  \ OAuth2 service remains fully available.\n\nerrors:\n  - status: 401\n    signal: 'WWW-Authenticate: Bearer error=\"invalid_token\", error_description=\"The access token expired\"'\n    applies_to: Marketing API\n    remediation: Refresh the access token with the refresh_token grant and retry.\n  - status: 401\n    signal: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.snapchat.com/.well-known/oauth-protected-resource/ads\"'\n    applies_to: Ads MCP\n    remediation: Complete the OAuth flow with the agent's pre-registered client id and scope snapads.read.\n\nnotes: >-\n  Many standard OAuth 2.0 client libraries handle the Marketing API\n  refresh-and-retry pattern automatically. The MCP server rejects the default\n  scope set requested by generic clients — Snap's own docs warn that the scope\n  must be exactly `snapads.read` or authorization fails.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/authentication/snap-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- Marketing
- Social-Media
- Augmented Reality
- Camera
- Authentication
- Identity
- Conversions
- Attribution
- SDK
---
