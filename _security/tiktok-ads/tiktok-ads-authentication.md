---
api_key_in:
- header
api_specs:
- filename: tiktok-ads-marketing-api-openapi.yml
  format: yaml
  label: TikTok Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-ads/refs/heads/main/openapi/tiktok-ads-marketing-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tiktok Ads Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TikTok Marketing API secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TikTok Marketing API
provider_slug: tiktok-ads
scheme_count: 2
schemes:
- description: Long-term access token for the Marketing API. Issued by POST /oauth2/access_token/ (Content-Type application/json) or POST /oauth/token/ (application/x-www-form-urlencoded), exchanging app_id + secret + auth_code. Sent on every subsequent request in the Access-Token request header.
  in: header
  name: AccessToken
  parameter: Access-Token
  sources:
  - openapi/tiktok-ads-marketing-api-openapi.yml
  spec_note: 'In the first-party OpenAPI fragments the token is declared as a QUERY parameter named Access-Token on every operation. The docs and every published curl example send it as a HEADER (--header ''Access-Token: ...''), and the 40104 error body returned by a live unauthenticated call says "you should set it in http header with key Access-Token". The header form is authoritative; the spec is wrong here, and this artifact records the header form.'
  surface: REST Marketing API
  type: apiKey
- dynamic_client_registration: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/register
  flows:
  - authorizationUrl: https://business-api.tiktok.com/portal/mcp-tt4b-authorize
    flow: authorizationCode
    scopes:
      mcp:tt4b: Act on TikTok Ads resources on behalf of the authorizing TikTok for Business user
    tokenUrl: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  jwks_uri: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/jwks
  name: MCPOAuth
  pkce:
  - S256
  revocation_endpoint: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/revoke
  sources:
  - well-known/tiktok-ads-oauth-authorization-server-mcp-flat.json
  - well-known/tiktok-ads-oauth-protected-resource-mcp-flat.json
  surface: TikTok for Business MCP Server
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: tiktok-ads-authentication
source_filename: tiktok-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/tiktok-ads-marketing-api-openapi.yml\ndocs: https://business-api.tiktok.com/portal/docs?id=1738373164380162\nauthorization_docs: https://business-api.tiktok.com/portal/docs?id=1738373141733378\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Two different auth systems live behind one brand. The REST Marketing API uses a three-legged\n    advertiser authorization that ends in a long-lived opaque token presented as a plain `Access-Token`\n    HEADER — not an OAuth bearer token, and not an Authorization header. The MCP server uses real OAuth\n    2.1: authorization code + PKCE, dynamic client registration, refresh tokens, and RFC 9728 / RFC 8414\n    discovery metadata that TikTok actually serves. An agent that can talk to the MCP server therefore has\n    a far more standard credential story than one calling the REST API directly.\nschemes:\n  - name: AccessToken\n\
  \    type: apiKey\n    in: header\n    parameter: Access-Token\n    surface: REST Marketing API\n    description: >-\n      Long-term access token for the Marketing API. Issued by POST /oauth2/access_token/ (Content-Type\n      application/json) or POST /oauth/token/ (application/x-www-form-urlencoded), exchanging app_id +\n      secret + auth_code. Sent on every subsequent request in the Access-Token request header.\n    sources: [openapi/tiktok-ads-marketing-api-openapi.yml]\n    spec_note: >-\n      In the first-party OpenAPI fragments the token is declared as a QUERY parameter named Access-Token on\n      every operation. The docs and every published curl example send it as a HEADER\n      (--header 'Access-Token: ...'), and the 40104 error body returned by a live unauthenticated call says\n      \"you should set it in http header with key Access-Token\". The header form is authoritative; the spec\n      is wrong here, and this artifact records the header form.\n  - name: MCPOAuth\n\
  \    type: oauth2\n    surface: TikTok for Business MCP Server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://business-api.tiktok.com/portal/mcp-tt4b-authorize\n        tokenUrl: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/token\n        scopes:\n          mcp:tt4b: Act on TikTok Ads resources on behalf of the authorizing TikTok for Business user\n    pkce: [S256]\n    dynamic_client_registration: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/register\n    revocation_endpoint: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/revoke\n    jwks_uri: https://business-api.tiktok.com/open_mcp/tt-ads-mcp-flat/oauth/jwks\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none]\n    sources:\n      - well-known/tiktok-ads-oauth-authorization-server-mcp-flat.json\n      - well-known/tiktok-ads-oauth-protected-resource-mcp-flat.json\nflow:\n  rest:\n    - Register as a developer\
  \ and create a developer app on the TikTok API for Business portal.\n    - Select the permission scope for the app (see scopes/tiktok-ads-scopes.yml).\n    - Send the app's Advertiser authorization URL to the advertiser; up to 10 redirect URLs may be configured, localhost included.\n    - The advertiser approves the permission list, agrees to the Platform Service Agreement, and confirms an emailed verification code.\n    - TikTok redirects to your redirect_uri with auth_code appended; auth_code is valid for 1 hour and single-use.\n    - POST app_id + secret + auth_code to /oauth2/access_token/ to receive access_token, advertiser_ids[] and the granted scope[].\n    - Send Access-Token on every subsequent request.\n  mcp:\n    - Point an MCP client at one of the two server URLs; no developer app or API key is required.\n    - The client is challenged with 401 + WWW-Authenticate carrying the RFC 9728 resource metadata URL.\n    - Standard OAuth authorization-code + PKCE flow against the discovered\
  \ authorization server, with dynamic client registration.\n    - The user signs in to TikTok Ads Manager and authorizes; the grant lasts 30 days and must then be renewed.\ntoken:\n  type: opaque\n  expiry: >-\n    The Marketing API long-term access token does not expire on a timer. It becomes invalid when the\n    advertiser cancels the authorization, or when it is explicitly revoked via /oauth2/revoke_token/.\n  revocation_endpoint: /oauth2/revoke_token/\n  refresh: not applicable for the long-term Marketing API token; the MCP OAuth token supports refresh_token\n  introspection_endpoint: /oauth2/advertiser/get/\n  introspection_note: returns the full list of advertiser accounts an access token can reach\n  scope_note: >-\n    The token carries only the permissions the ADVERTISER granted, which may be narrower than the\n    permissions the developer app requested.\nverification:\n  advertiser_reauth_window_hours: 48\n  note: >-\n    An ad account that has already authorized a given developer\
  \ app does not have to re-verify by email for\n    48 hours. Authorizing a DIFFERENT developer app always requires a fresh verification.\nsandbox:\n  base_url: https://sandbox-ads.tiktok.com/open_api\n  note: sandbox access tokens are generated per developer app; see sandbox/tiktok-ads-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiktok-ads/refs/heads/main/authentication/tiktok-ads-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Advertising
- Marketing
- Social Media
- Ad Campaigns
- Performance Marketing
- Conversion Tracking
- Audience Management
- Reporting
- Product Catalog
- Agent Ready
---
