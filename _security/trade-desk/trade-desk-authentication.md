---
api_key_in:
- header
api_specs:
- filename: trade-desk-advertiser-api-openapi.yml
  format: yaml
  label: The Trade Desk Advertiser API
  slug: trade-desk-advertiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-advertiser-api-openapi.yml
- filename: trade-desk-deletionoptout-api-openapi.yml
  format: yaml
  label: The Trade Desk DeletionOptOut API
  slug: trade-desk-deletionoptout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-deletionoptout-api-openapi.yml
- filename: trade-desk-offlineconversion-api-openapi.yml
  format: yaml
  label: The Trade Desk OfflineConversion API
  slug: trade-desk-offlineconversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-offlineconversion-api-openapi.yml
- filename: trade-desk-thirdparty-api-openapi.yml
  format: yaml
  label: The Trade Desk ThirdParty API
  slug: trade-desk-thirdparty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-thirdparty-api-openapi.yml
- filename: trade-desk-ipaddress-api-openapi.yml
  format: yaml
  label: The Trade Desk IPAddress Data API
  slug: trade-desk-ipaddress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-ipaddress-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Trade Desk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- password
- implicit
- ciba
overview: The Trade Desk secures its APIs with apiKey, oauth2, openIdConnect, and http across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, password, implicit, and ciba flow(s).
provider_name: The Trade Desk
provider_slug: trade-desk
scheme_count: 7
schemes:
- description: Platform API token. Used by the Platform REST API, the Platform GraphQL API, the Workflows API, the Data API and the OAK MCP server — one token type across the whole surface.
  docs: https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/PlatformAuthentication
  in: header
  issuance: https://open.thetradedesk.com/advertiser/access-management
  name: TTD-Auth
  parameter: TTD-Auth
  primary: true
  rotation: Tokens cannot be updated. To change a lifetime you revoke, generate a new token, and replace it in the integration. Short-lived tokens cannot be revoked at all — they expire only.
  sources:
  - openapi/_original/trade-desk-data-api-swagger.json
  - openapi/trade-desk-advertiser-api-openapi.yml
  token_lifetime: One week to one year when generated in the OpenTTD Access Management UI; up to 24 hours (1440 minutes) when generated via POST /v3/authentication.
  type: apiKey
- description: 'POST /v3/authentication with Login + Password (and optional TokenExpirationInMinutes, default 1440) returns {"Token": "..."} for use as the TTD-Auth header value. Maximum 24 hours. Documented as non-revocable and intended for temporary or low-risk use, not production.'
  endpoint: https://api.thetradedesk.com/v3/authentication
  name: ShortLivedToken
  scheme: custom
  sources:
  - https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/AuthenticationShortLive
  type: http
- description: Full OIDC provider fronting the platform. 92 scopes, RS256 id_token signing, PKCE (S256), private_key_jwt client auth, device-code and CIBA grants. This is the authorization server named by the MCP protected-resource metadata.
  name: OpenIDConnect
  openIdConnectUrl: https://auth.thetradedesk.com/.well-known/openid-configuration
  scopes: scopes/trade-desk-scopes.yml
  sources:
  - https://auth.thetradedesk.com/.well-known/openid-configuration
  type: openIdConnect
- description: OAuth is offered for the OAK MCP server as the no-manual-token-management path; OIDC token exchange is available on request for teams building applications on top of OAK.
  flows:
  - authorizationUrl: https://auth.thetradedesk.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://auth.thetradedesk.com/connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.thetradedesk.com/connect/token
  name: OAuth2
  sources:
  - https://api.thetradedesk.com/.well-known/oauth-protected-resource/mcp/platform-management
  type: oauth2
- deprecated: true
  description: LEGACY Data API auth. HMAC-SHA1 base64 of the JSON request body keyed with the advertiser secret key (audience data) or the data-provider secret key (offline conversions). The provider now directs all Data API traffic to token authentication.
  in: header
  name: TtdSignature
  parameter: TtdSignature
  sources:
  - https://open.thetradedesk.com/advertiser/docsApp/GuidesAdvertiser/data/doc/DataApiCallsAdvertiser
  type: apiKey
- applies_to: https://open.sincera.io/api
  description: 'OpenSincera API uses Authorization: Bearer with a personal API key retrieved from the OpenSincera profile page. Separate account and separate credential from the Platform API.'
  name: SinceraBearer
  scheme: bearer
  sources:
  - https://open.thetradedesk.com/seller/docsApp/GuidesSeller/opensincera/doc/OpenSinceraGetStarted
  type: http
- description: The Real-Time Conversion Events endpoint (POST https://insight.adsrvr.org/track/realtimeconversion) is documented as requiring no authentication.
  name: None
  sources:
  - https://open.thetradedesk.com/advertiser/docsApp/GuidesAdvertiser/data/doc/post-track-realtimeconversion
  type: none
slug: trade-desk-authentication
source_filename: trade-desk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/trade-desk-data-api-swagger.json + provider docs\ndocs:\n- https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/PlatformAuthentication\n- https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/AuthenticationShortLive\n- https://open.thetradedesk.com/advertiser/docsApp/GuidesAdvertiser/data/doc/DataApiCallsAdvertiser\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  - http\n  api_key_in:\n  - header\n  api_key_names:\n  - TTD-Auth\n  - TtdSignature\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - password\n  - implicit\n  - ciba\n  issuer: https://auth.thetradedesk.com\nschemes:\n- name: TTD-Auth\n  type: apiKey\n  in: header\n  parameter: TTD-Auth\n  primary: true\n  sources:\n  - openapi/_original/trade-desk-data-api-swagger.json\n  - openapi/trade-desk-advertiser-api-openapi.yml\n  description: Platform API token.\
  \ Used by the Platform REST API, the Platform GraphQL API, the Workflows\n    API, the Data API and the OAK MCP server — one token type across the whole surface.\n  token_lifetime: One week to one year when generated in the OpenTTD Access Management UI; up to 24 hours\n    (1440 minutes) when generated via POST /v3/authentication.\n  issuance: https://open.thetradedesk.com/advertiser/access-management\n  rotation: Tokens cannot be updated. To change a lifetime you revoke, generate a new token, and replace\n    it in the integration. Short-lived tokens cannot be revoked at all — they expire only.\n  docs: https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/PlatformAuthentication\n- name: ShortLivedToken\n  type: http\n  scheme: custom\n  sources:\n  - https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/AuthenticationShortLive\n  description: 'POST /v3/authentication with Login + Password (and optional TokenExpirationInMinutes,\n    default 1440)\
  \ returns {\"Token\": \"...\"} for use as the TTD-Auth header value. Maximum 24 hours. Documented\n    as non-revocable and intended for temporary or low-risk use, not production.'\n  endpoint: https://api.thetradedesk.com/v3/authentication\n- name: OpenIDConnect\n  type: openIdConnect\n  sources:\n  - https://auth.thetradedesk.com/.well-known/openid-configuration\n  openIdConnectUrl: https://auth.thetradedesk.com/.well-known/openid-configuration\n  description: Full OIDC provider fronting the platform. 92 scopes, RS256 id_token signing, PKCE (S256),\n    private_key_jwt client auth, device-code and CIBA grants. This is the authorization server named by\n    the MCP protected-resource metadata.\n  scopes: scopes/trade-desk-scopes.yml\n- name: OAuth2\n  type: oauth2\n  sources:\n  - https://api.thetradedesk.com/.well-known/oauth-protected-resource/mcp/platform-management\n  description: OAuth is offered for the OAK MCP server as the no-manual-token-management path; OIDC token\n    exchange\
  \ is available on request for teams building applications on top of OAK.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.thetradedesk.com/connect/authorize\n    tokenUrl: https://auth.thetradedesk.com/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.thetradedesk.com/connect/token\n- name: TtdSignature\n  type: apiKey\n  in: header\n  parameter: TtdSignature\n  deprecated: true\n  sources:\n  - https://open.thetradedesk.com/advertiser/docsApp/GuidesAdvertiser/data/doc/DataApiCallsAdvertiser\n  description: LEGACY Data API auth. HMAC-SHA1 base64 of the JSON request body keyed with the advertiser\n    secret key (audience data) or the data-provider secret key (offline conversions). The provider now\n    directs all Data API traffic to token authentication.\n- name: SinceraBearer\n  type: http\n  scheme: bearer\n  sources:\n  - https://open.thetradedesk.com/seller/docsApp/GuidesSeller/opensincera/doc/OpenSinceraGetStarted\n  description: 'OpenSincera\
  \ API uses Authorization: Bearer with a personal API key retrieved from the\n    OpenSincera profile page. Separate account and separate credential from the Platform API.'\n  applies_to: https://open.sincera.io/api\n- name: None\n  type: none\n  sources:\n  - https://open.thetradedesk.com/advertiser/docsApp/GuidesAdvertiser/data/doc/post-track-realtimeconversion\n  description: The Real-Time Conversion Events endpoint (POST https://insight.adsrvr.org/track/realtimeconversion)\n    is documented as requiring no authentication.\ngaps:\n- No securityScheme is declared in any published OpenAPI — the Data API spec models TTD-Auth as a required\n  header PARAMETER on every operation instead of as a securityScheme, so machine clients get no auth affordance\n  from the contract.\n- No public scopes/permissions reference page; the 92 scopes are discoverable only from the OIDC discovery\n  document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/authentication/trade-desk-authentication.yml
summary_line: apiKey/oauth2/openIdConnect/http · 7 schemes
tags:
- Advertising
- Programmatic Advertising
- Demand-Side Platform
- DSP
- AdTech
- Connected TV
- CTV
- Identity
- Unified ID 2.0
- UID2
- OpenPath
- Kokai
- Koa AI
- Galileo
- Sincera
- Open Internet
- Real-Time Bidding
- Open Measurement
---
