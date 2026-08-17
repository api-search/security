---
api_key_in:
- query
api_specs:
- filename: snapchat-ads-api-openapi.yml
  format: yaml
  label: Snapchat Ads API
  slug: snapchat-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ads-api-openapi.yml
- filename: snapchat-ad-accounts-api-openapi.yml
  format: yaml
  label: Snapchat Ad Accounts API
  slug: snapchat-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-accounts-api-openapi.yml
- filename: snapchat-ad-squads-api-openapi.yml
  format: yaml
  label: Snapchat Ad Squads API
  slug: snapchat-ad-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-squads-api-openapi.yml
- filename: snapchat-audience-segments-api-openapi.yml
  format: yaml
  label: Snapchat Audience Segments API
  slug: snapchat-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-audience-segments-api-openapi.yml
- filename: snapchat-campaigns-api-openapi.yml
  format: yaml
  label: Snapchat Campaigns API
  slug: snapchat-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-campaigns-api-openapi.yml
- filename: snapchat-conversion-events-api-openapi.yml
  format: yaml
  label: Snapchat Conversion Events API
  slug: snapchat-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversion-events-api-openapi.yml
- filename: snapchat-creatives-api-openapi.yml
  format: yaml
  label: Snapchat Creatives API
  slug: snapchat-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-creatives-api-openapi.yml
- filename: snapchat-funding-sources-api-openapi.yml
  format: yaml
  label: Snapchat Funding Sources API
  slug: snapchat-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-funding-sources-api-openapi.yml
- filename: snapchat-measurement-api-openapi.yml
  format: yaml
  label: Snapchat Measurement API
  slug: snapchat-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-measurement-api-openapi.yml
- filename: snapchat-media-api-openapi.yml
  format: yaml
  label: Snapchat Media API
  slug: snapchat-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-media-api-openapi.yml
- filename: snapchat-oauth-api-openapi.yml
  format: yaml
  label: Snapchat OAuth API
  slug: snapchat-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-oauth-api-openapi.yml
- filename: snapchat-organizations-api-openapi.yml
  format: yaml
  label: Snapchat Organizations API
  slug: snapchat-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-organizations-api-openapi.yml
- filename: snapchat-user-profile-api-openapi.yml
  format: yaml
  label: Snapchat User Profile API
  slug: snapchat-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-user-profile-api-openapi.yml
auth_types:
- oauth2
- http
- apiKey
description: Every Snapchat developer surface authenticates with OAuth 2.0, but through three different authorization servers with three different token shapes. The Marketing API and Login Kit both go through accounts.snapchat.com; the Ads MCP server runs its own authorization server at mcp.snapchat.com with pre-registered per-vendor client ids and a single read scope. The Conversions API additionally accepts a long-lived static token generated in Ads Manager and passed as a QUERY PARAMETER, which is the weakest link in the set — it puts a credential in URLs, logs and referrers.
kind: authentication
layout: security
method: searched
name: Snapchat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refresh_token
overview: Snapchat secures its APIs with oauth2, http, and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and refresh_token flow(s).
provider_name: Snapchat
provider_slug: snapchat
scheme_count: 5
schemes:
- description: OAuth 2.0 authorization code flow. Access tokens expire after 3600 seconds; refresh tokens obtain new ones. The token reflects the authorizing user's Business Manager permissions, so API calls are scoped to what that user can already access.
  flows:
  - authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth
    flow: authorizationCode
    refreshUrl: https://accounts.snapchat.com/login/oauth2/access_token
    scopes:
    - snapchat-marketing-api
    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token
  header: 'Authorization: Bearer <access_token>'
  name: bearerAuth
  product: Snapchat Marketing API
  refresh: true
  sources:
  - openapi/snapchat-ads-api-openapi.yml
  - https://developers.snap.com/marketing-api/Ads-API/authentication
  token_ttl_seconds: 3600
  type: oauth2
- app_management: https://kit.snapchat.com/manage/apps
  description: Snap's implementation of OAuth 2.0 for "Log in with Snapchat". The Login Kit SDKs are being deprecated; the OAuth 2.0 service behind them remains fully supported. Returns no id_token — identity is read from GET /me on kit.snapchat.com.
  flows:
  - authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth
    flow: authorizationCode
    pkce: required for public clients (code_challenge_method=S256)
    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token
  - flow: authorizationCode
    variant: server-side (confidential client with client_secret, long-term refresh tokens)
  - flow: implicit
    note: Snap documents this as "limited security compared to other flows".
    variant: response_type=token for SPAs
  name: loginKitOAuth
  product: Login Kit
  required_parameters:
  - client_id
  - redirect_uri
  - response_type
  - scope
  - state
  - code_challenge
  - code_challenge_method
  sources:
  - openapi/_original/snapchat-login-kit-openapi.yml
  - https://developers.snap.com/snap-kit/login-kit/overview
  type: oauth2
- description: 'Separate authorization server for the hosted MCP endpoint. Client ids are registered by Snap per agent vendor (claude-snap-ads, codex-snap-ads, chatgpt-snap-ads, antigravity-snap-ads, gemini-snap-ads) — advertisers cannot register their own, and other client ids are rejected. Approval is two-stage: an org Admin or Business Admin approves the agent for the organization, then each member authorizes individually.'
  dynamic_client_registration: false
  flows:
  - authorizationUrl: https://mcp.snapchat.com/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
    - snapads.read
    tokenUrl: https://mcp.snapchat.com/token
  name: mcpOAuth
  product: Snapchat Ads MCP Server
  resource: https://mcp.snapchat.com/ads
  revocation: https://accounts.snapchat.com/v2/manage-apps
  sources:
  - https://developers.snap.com/marketing-api/Ads-MCP/Introduction
  - https://mcp.snapchat.com/.well-known/oauth-authorization-server/ads
  token_endpoint_auth_method: none
  type: oauth2
- description: Static long-lived access token generated from the Business Details page of Ads Manager, passed as a query parameter. Accepted alongside OAuth bearer tokens on the Conversions API and its /events/validate test endpoint, provided the pixel or app is owned by the organization that generated the token.
  in: query
  name: accessToken
  parameter: access_token
  product: Snapchat Conversions API
  risk: A long-lived bearer credential in a URL leaks into access logs, browser history and Referer headers. Prefer the OAuth flow where the integration can support it.
  sources:
  - openapi/_original/snapchat-conversions-api-openapi.yml
  - https://developers.snap.com/marketing-api/Conversions-API/GetStarted
  type: apiKey
- description: Bearer access token from the Login Kit OAuth flow, used against https://kit.snapchat.com/v1/me.
  name: bearerAuth
  product: Login Kit profile API
  scheme: bearer
  sources:
  - openapi/_original/snapchat-login-kit-openapi.yml
  type: http
slug: snapchat-authentication
source_filename: snapchat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.snap.com/marketing-api/Ads-API/authentication,\n  https://developers.snap.com/snap-kit/login-kit/overview,\n  https://developers.snap.com/marketing-api/Ads-MCP/Introduction,\n  https://mcp.snapchat.com/.well-known/oauth-authorization-server/ads,\n  openapi/*.yml, openapi/_original/*.yml\ndocs:\n- https://developers.snap.com/marketing-api/Ads-API/authentication\n- https://developers.snap.com/snap-kit/login-kit/overview\nprovider: Snapchat\nproviderId: snapchat\ndescription: >-\n  Every Snapchat developer surface authenticates with OAuth 2.0, but through three different\n  authorization servers with three different token shapes. The Marketing API and Login Kit both go\n  through accounts.snapchat.com; the Ads MCP server runs its own authorization server at\n  mcp.snapchat.com with pre-registered per-vendor client ids and a single read scope. The\n  Conversions API additionally accepts a long-lived static\
  \ token generated in Ads Manager and\n  passed as a QUERY PARAMETER, which is the weakest link in the set — it puts a credential in URLs,\n  logs and referrers.\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refresh_token\n  pkce: S256\n  openid_connect: false\n  mtls: false\nschemes:\n- name: bearerAuth\n  type: oauth2\n  product: Snapchat Marketing API\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth\n    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token\n    refreshUrl: https://accounts.snapchat.com/login/oauth2/access_token\n    scopes:\n    - snapchat-marketing-api\n  header: 'Authorization: Bearer <access_token>'\n  token_ttl_seconds: 3600\n  refresh: true\n  description: >-\n    OAuth 2.0 authorization code flow. Access tokens expire after 3600 seconds; refresh tokens\n    obtain new ones. The token reflects the\
  \ authorizing user's Business Manager permissions, so API\n    calls are scoped to what that user can already access.\n  sources:\n  - openapi/snapchat-ads-api-openapi.yml\n  - https://developers.snap.com/marketing-api/Ads-API/authentication\n- name: loginKitOAuth\n  type: oauth2\n  product: Login Kit\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth\n    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token\n    pkce: required for public clients (code_challenge_method=S256)\n  - flow: authorizationCode\n    variant: server-side (confidential client with client_secret, long-term refresh tokens)\n  - flow: implicit\n    variant: response_type=token for SPAs\n    note: Snap documents this as \"limited security compared to other flows\".\n  required_parameters:\n  - client_id\n  - redirect_uri\n  - response_type\n  - scope\n  - state\n  - code_challenge\n  - code_challenge_method\n  app_management: https://kit.snapchat.com/manage/apps\n\
  \  description: >-\n    Snap's implementation of OAuth 2.0 for \"Log in with Snapchat\". The Login Kit SDKs are being\n    deprecated; the OAuth 2.0 service behind them remains fully supported. Returns no id_token —\n    identity is read from GET /me on kit.snapchat.com.\n  sources:\n  - openapi/_original/snapchat-login-kit-openapi.yml\n  - https://developers.snap.com/snap-kit/login-kit/overview\n- name: mcpOAuth\n  type: oauth2\n  product: Snapchat Ads MCP Server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.snapchat.com/authorize\n    tokenUrl: https://mcp.snapchat.com/token\n    pkce: S256\n    scopes:\n    - snapads.read\n  resource: https://mcp.snapchat.com/ads\n  token_endpoint_auth_method: none\n  dynamic_client_registration: false\n  description: >-\n    Separate authorization server for the hosted MCP endpoint. Client ids are registered by Snap per\n    agent vendor (claude-snap-ads, codex-snap-ads, chatgpt-snap-ads, antigravity-snap-ads,\n    gemini-snap-ads)\
  \ — advertisers cannot register their own, and other client ids are rejected.\n    Approval is two-stage: an org Admin or Business Admin approves the agent for the organization,\n    then each member authorizes individually.\n  revocation: https://accounts.snapchat.com/v2/manage-apps\n  sources:\n  - https://developers.snap.com/marketing-api/Ads-MCP/Introduction\n  - https://mcp.snapchat.com/.well-known/oauth-authorization-server/ads\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: access_token\n  product: Snapchat Conversions API\n  description: >-\n    Static long-lived access token generated from the Business Details page of Ads Manager, passed\n    as a query parameter. Accepted alongside OAuth bearer tokens on the Conversions API and its\n    /events/validate test endpoint, provided the pixel or app is owned by the organization that\n    generated the token.\n  risk: >-\n    A long-lived bearer credential in a URL leaks into access logs, browser history and Referer\n\
  \    headers. Prefer the OAuth flow where the integration can support it.\n  sources:\n  - openapi/_original/snapchat-conversions-api-openapi.yml\n  - https://developers.snap.com/marketing-api/Conversions-API/GetStarted\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  product: Login Kit profile API\n  description: Bearer access token from the Login Kit OAuth flow, used against https://kit.snapchat.com/v1/me.\n  sources:\n  - openapi/_original/snapchat-login-kit-openapi.yml\nscopes: scopes/snapchat-scopes.yml\nnotes:\n- No OpenID Connect layer. /.well-known/openid-configuration 404s on accounts.snapchat.com, snapchat.com and mcp.snapchat.com.\n- No mutual TLS, no HTTP signature scheme, no request signing.\n- >-\n  Roles, not scopes, carry most Marketing API authorization. Business Manager roles (including\n  agency_admin and agency_member, added 2026-07-01) determine what an authorized token can reach.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/authentication/snapchat-authentication.yml
summary_line: oauth2/http/apiKey · 5 schemes
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social Media
---
