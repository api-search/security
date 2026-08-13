---
api_key_in:
- header
auth_types:
- placement-code
- app-id
- token
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Madvertise Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Madvertise secures its APIs with placement-code, app-id, token, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Madvertise
provider_slug: madvertise
scheme_count: 4
schemes:
- detail: Ad requests carry the zone/publisher/placement ID in the `s` query parameter (mobile.mng-ads.com) or the URL path (/bidrequest/{placement_code}). This identifies inventory, not an authenticated principal — anyone who knows a placement code can issue a bid request against it. No key, token, signature or mTLS is documented.
  location: query-or-path
  name: placement-code
  source: https://developers.bluestack.app/adserving/ad-request-api-documentation
  surface: ad-serving
  type: identifier
- detail: Mobile SDKs initialize with a publisher appID via MobileAds.sharedInstance() (iOS) / SDK init (Android) before loading ads.
  location: sdk-init
  name: app-id
  source: https://developers.bluestack.app/ios/
  surface: mobile-sdk
  type: identifier
- detail: '"Use the token returned by auth-reporting service when making calls to /seller-reporting, /buyer-reporting and /mediation-reporting." The token is an opaque 40-character hex string sent bare in the Authorization header — NOT prefixed with "Bearer", per the docs'' own curl examples (`-H ''Authorization: fbe74e915898ee0d560643d0f3dd722eb17bade3''`). No expiry, refresh, rotation or revocation semantics are documented, and no scopes exist.'
  gate_detail: 'The reporting host itself is withheld: "All API access is over HTTPS, and accessed via the https://xxx.com domain (ask to your Azerion contact)." The reference is public but the base URL is issued only to contracted partners.'
  gated: true
  location: header
  name: reporting-token
  parameter_name: Authorization
  scheme: token
  source: https://developers.bluestack.app/reporting/seller-reporting-api
  surface: reporting
  token_endpoint: POST /auth-reporting
  type: http
- detail: Azerion's Improve Digital publisher MCP server authenticates to api.360yield.com with OAuth2 client credentials (IMPROVE_DIGITAL_CLIENT_ID / _CLIENT_SECRET) and manages bearer-token expiry internally. Recorded for completeness because it is the only OAuth2 anywhere in this estate; it does not apply to the mng-ads.com APIs. No token URL or scope list is published, so no scopes/ artifact is emitted.
  flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: null
  name: improvedigital-oauth2
  source: https://github.com/azerion/improvedigital-publisher-mcp-server
  surface: sibling (Improve Digital 360Yield publisher inventory — NOT Madvertise ad serving)
  type: oauth2
slug: madvertise-authentication
source_filename: madvertise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://developers.bluestack.app/adserving/ad-request-api-documentation,\n  https://developers.bluestack.app/adserving/open-rtb-bid-request-api,\n  https://developers.bluestack.app/reporting/seller-reporting-api,\n  https://developers.bluestack.app/reporting/buyer-reporting-api,\n  https://developers.bluestack.app/reporting/mediation-reporting-api,\n  https://developers.bluestack.app/android/,\n  https://github.com/azerion/improvedigital-publisher-mcp-server\nnote: >-\n  No OpenAPI is published for any Madvertise-branded API, so this profile is captured\n  from the developer docs rather than derived. Madvertise runs THREE distinct and\n  unrelated identity models, which is the single most important thing for an agent to\n  know about this provider: the ad-serving APIs are unauthenticated and identify\n  inventory by placement code; the reporting APIs use a bearer-style opaque token minted\n  by a dedicated /auth-reporting\
  \ endpoint; and Azerion's sibling Improve Digital MCP\n  server uses OAuth2 client credentials against a different host entirely.\nsummary:\n  types: [placement-code, app-id, token, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: placement-code\n  type: identifier\n  surface: ad-serving\n  location: query-or-path\n  detail: >-\n    Ad requests carry the zone/publisher/placement ID in the `s` query parameter\n    (mobile.mng-ads.com) or the URL path (/bidrequest/{placement_code}). This identifies\n    inventory, not an authenticated principal — anyone who knows a placement code can\n    issue a bid request against it. No key, token, signature or mTLS is documented.\n  source: https://developers.bluestack.app/adserving/ad-request-api-documentation\n- name: app-id\n  type: identifier\n  surface: mobile-sdk\n  location: sdk-init\n  detail: >-\n    Mobile SDKs initialize with a publisher appID via MobileAds.sharedInstance() (iOS) /\n    SDK init (Android)\
  \ before loading ads.\n  source: https://developers.bluestack.app/ios/\n- name: reporting-token\n  type: http\n  scheme: token\n  surface: reporting\n  location: header\n  parameter_name: Authorization\n  token_endpoint: POST /auth-reporting\n  detail: >-\n    \"Use the token returned by auth-reporting service when making calls to\n    /seller-reporting, /buyer-reporting and /mediation-reporting.\" The token is an\n    opaque 40-character hex string sent bare in the Authorization header — NOT prefixed\n    with \"Bearer\", per the docs' own curl examples\n    (`-H 'Authorization: fbe74e915898ee0d560643d0f3dd722eb17bade3'`). No expiry,\n    refresh, rotation or revocation semantics are documented, and no scopes exist.\n  gated: true\n  gate_detail: >-\n    The reporting host itself is withheld: \"All API access is over HTTPS, and accessed\n    via the https://xxx.com domain (ask to your Azerion contact).\" The reference is\n    public but the base URL is issued only to contracted partners.\n\
  \  source: https://developers.bluestack.app/reporting/seller-reporting-api\n- name: improvedigital-oauth2\n  type: oauth2\n  surface: sibling (Improve Digital 360Yield publisher inventory — NOT Madvertise ad serving)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    scopes: {}\n  detail: >-\n    Azerion's Improve Digital publisher MCP server authenticates to api.360yield.com\n    with OAuth2 client credentials (IMPROVE_DIGITAL_CLIENT_ID / _CLIENT_SECRET) and\n    manages bearer-token expiry internally. Recorded for completeness because it is the\n    only OAuth2 anywhere in this estate; it does not apply to the mng-ads.com APIs. No\n    token URL or scope list is published, so no scopes/ artifact is emitted.\n  source: https://github.com/azerion/improvedigital-publisher-mcp-server\ngaps:\n- No API key, token or signature on the OpenRTB bid-request endpoint — a placement code\n  is the whole credential.\n- No published scope model anywhere; the reporting token is all-or-nothing\
  \ per account.\n- No token lifetime, rotation or revocation documented for /auth-reporting.\n- No /.well-known/oauth-authorization-server or openid-configuration on any host\n  (see well-known/madvertise-well-known.yml).\ncross_links:\n  conventions: conventions/madvertise-conventions.yml\n  mcp: mcp/madvertise-mcp.yml\n  well_known: well-known/madvertise-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madvertise/refs/heads/main/authentication/madvertise-authentication.yml
summary_line: placement-code/app-id/token/oauth2 · 4 schemes
tags:
- Company
- Advertising
- AdTech
- Mobile
- Monetization
- Programmatic
- OpenRTB
- SDK
- Publishers
---
