---
api_key_in: []
api_specs:
- filename: facebook-business-manager-ad-accounts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Accounts API
  slug: facebook-business-manager-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-accounts-api-openapi.yml
- filename: facebook-business-manager-ad-creatives-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Creatives API
  slug: facebook-business-manager-ad-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-creatives-api-openapi.yml
- filename: facebook-business-manager-ad-images-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Images API
  slug: facebook-business-manager-ad-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-images-api-openapi.yml
- filename: facebook-business-manager-ad-sets-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Sets API
  slug: facebook-business-manager-ad-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-sets-api-openapi.yml
- filename: facebook-business-manager-ads-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ads API
  slug: facebook-business-manager-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ads-api-openapi.yml
- filename: facebook-business-manager-campaigns-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Campaigns API
  slug: facebook-business-manager-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-campaigns-api-openapi.yml
- filename: facebook-business-manager-comments-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Comments API
  slug: facebook-business-manager-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-comments-api-openapi.yml
- filename: facebook-business-manager-custom-audiences-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Custom Audiences API
  slug: facebook-business-manager-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-custom-audiences-api-openapi.yml
- filename: facebook-business-manager-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Insights API
  slug: facebook-business-manager-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-insights-api-openapi.yml
- filename: facebook-business-manager-page-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Page Insights API
  slug: facebook-business-manager-page-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-page-insights-api-openapi.yml
- filename: facebook-business-manager-pages-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Pages API
  slug: facebook-business-manager-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-pages-api-openapi.yml
- filename: facebook-business-manager-photos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Photos API
  slug: facebook-business-manager-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-photos-api-openapi.yml
- filename: facebook-business-manager-posts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Posts API
  slug: facebook-business-manager-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-posts-api-openapi.yml
- filename: facebook-business-manager-videos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Videos API
  slug: facebook-business-manager-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-videos-api-openapi.yml
auth_types:
- oauth2
- http
- openIdConnect
description: 'Every Business Manager surface authenticates the same way: an OAuth 2.0 bearer access token issued through Facebook Login, scoped by user-granted permissions. The OpenAPI files in this repo declare only a generic http/bearer scheme; this file upgrades that thin derivation with what Meta actually documents — five distinct token types with materially different lifetimes and rate-limit regimes, an OIDC discovery document served at www.facebook.com, and an appsecret_proof signature for server-side calls. Upgraded 2026-08-13 from method: derived (openapi only) to method: searched.'
kind: authentication
layout: security
method: searched
name: Facebook Business Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facebook Business Manager secures its APIs with oauth2, http, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Facebook Business Manager
provider_slug: facebook-business-manager
scheme_count: 3
schemes:
- description: 'OAuth 2.0 access token presented as `Authorization: Bearer {token}` or as an `access_token` query parameter. This is the scheme the OpenAPI files declare.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/facebook-marketing-openapi.yml
  - openapi/facebook-pages-openapi.yml
  type: http
- description: Facebook Login. Scopes are Meta "permissions", requested at the dialog and grantable or deniable individually by the app user. Advanced Access to any permission requires App Review plus Business Verification.
  flows:
    authorizationCode:
      authorizationUrl: https://www.facebook.com/v26.0/dialog/oauth
      scopes_reference: scopes/facebook-business-manager-scopes.yml
      tokenUrl: https://graph.facebook.com/v26.0/oauth/access_token
  method: searched
  name: facebookLogin
  type: oauth2
- description: OIDC discovery document served live (HTTP 200, probed 2026-08-13). issuer https://www.facebook.com, authorization_endpoint https://facebook.com/dialog/oauth/, jwks_uri https://www.facebook.com/.well-known/oauth/openid/jwks/, id_token signing RS256, pairwise subject types. response_types_supported is [id_token, token id_token] only — no `code`. No userinfo_endpoint is advertised; profile claims are read from the Graph API /me node instead.
  file: well-known/facebook-business-manager-openid-configuration.json
  method: probed
  name: facebookOIDC
  openIdConnectUrl: https://www.facebook.com/.well-known/openid-configuration
  type: openIdConnect
slug: facebook-business-manager-authentication
source_filename: facebook-business-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.facebook.com/docs/facebook-login/guides/access-tokens\ndocs:\n  - https://developers.facebook.com/docs/facebook-login/guides/access-tokens\n  - https://developers.facebook.com/docs/permissions\n  - https://www.facebook.com/.well-known/openid-configuration\n  - https://mcp.facebook.com/.well-known/oauth-protected-resource/ads\nderived_from:\n  - openapi/facebook-marketing-openapi.yml\n  - openapi/facebook-pages-openapi.yml\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Facebook Business Manager\nproviderId: facebook-business-manager\ndescription: >-\n  Every Business Manager surface authenticates the same way: an OAuth 2.0 bearer access token issued through\n  Facebook Login, scoped by user-granted permissions. The OpenAPI files in this repo declare only a generic\n  http/bearer scheme; this file upgrades that thin derivation with what Meta actually documents — five\n  distinct\
  \ token types with materially different lifetimes and rate-limit regimes, an OIDC discovery document\n  served at www.facebook.com, and an appsecret_proof signature for server-side calls.\n  Upgraded 2026-08-13 from method: derived (openapi only) to method: searched.\nsummary:\n  types:\n    - oauth2\n    - http\n    - openIdConnect\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      OAuth 2.0 access token presented as `Authorization: Bearer {token}` or as an `access_token` query\n      parameter. This is the scheme the OpenAPI files declare.\n    sources:\n      - openapi/facebook-marketing-openapi.yml\n      - openapi/facebook-pages-openapi.yml\n  - name: facebookLogin\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://www.facebook.com/v26.0/dialog/oauth\n        tokenUrl: https://graph.facebook.com/v26.0/oauth/access_token\n        scopes_reference: scopes/facebook-business-manager-scopes.yml\n    description:\
  \ >-\n      Facebook Login. Scopes are Meta \"permissions\", requested at the dialog and grantable or deniable\n      individually by the app user. Advanced Access to any permission requires App Review plus Business\n      Verification.\n    method: searched\n  - name: facebookOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://www.facebook.com/.well-known/openid-configuration\n    description: >-\n      OIDC discovery document served live (HTTP 200, probed 2026-08-13). issuer https://www.facebook.com,\n      authorization_endpoint https://facebook.com/dialog/oauth/, jwks_uri\n      https://www.facebook.com/.well-known/oauth/openid/jwks/, id_token signing RS256, pairwise subject\n      types. response_types_supported is [id_token, token id_token] only — no `code`. No userinfo_endpoint is\n      advertised; profile claims are read from the Graph API /me node instead.\n    method: probed\n    file: well-known/facebook-business-manager-openid-configuration.json\ntoken_types:\n  -\
  \ name: User access token\n    obtained_via: Facebook Login dialog\n    lifetime: >-\n      Short-lived (~1-2 hours) by default; exchangeable for a long-lived token (~60 days) via\n      grant_type=fb_exchange_token.\n    rate_limit_regime: Platform Rate Limits\n  - name: Page access token\n    obtained_via: 'GET /me/accounts with pages_show_list (returns each Page''s own access_token)'\n    lifetime: Inherits the lifetime of the user token it was derived from; never-expiring when derived from a long-lived token.\n    rate_limit_regime: Business Use Case Rate Limits\n    note: >-\n      Page edges require a PAGE token, not the user token from Login. Using the user token is the single most\n      common silent authorization failure on the Pages surface.\n  - name: App access token\n    obtained_via: 'client_credentials, or the literal {app-id}|{app-secret} form'\n    lifetime: Does not expire until the app secret is rotated.\n    rate_limit_regime: Platform Rate Limits\n    note: Server-side\
  \ only. Never ship an app access token to a client.\n  - name: System user access token\n    obtained_via: Business Manager > Business Settings > System Users\n    lifetime: Non-expiring\n    rate_limit_regime: Business Use Case Rate Limits\n    note: >-\n      The right credential for unattended server-to-server automation. Not tied to a human account, so it\n      does not break when an employee leaves or when the 90-day permission decay fires.\n  - name: Client token\n    obtained_via: App Dashboard > Settings > Advanced\n    lifetime: Static\n    note: Limited-privilege identifier for mobile/web clients; not a substitute for a user token.\nrequest_signing:\n  name: appsecret_proof\n  algorithm: HMAC-SHA256 of the access token, keyed by the app secret, hex-encoded\n  transport: appsecret_proof query parameter (with appsecret_time)\n  required: false\n  note: >-\n    Recommended for all server-side calls. Prevents a stolen access token being replayed by a different app.\n    Can be made\
  \ mandatory per app in the App Dashboard.\ntoken_introspection:\n  endpoint: 'GET /debug_token?input_token={token}&access_token={app-token}'\n  tool: https://developers.facebook.com/tools/debug/accesstoken/\n  returns: app_id, type, application, expires_at, is_valid, scopes granted, user_id\nmcp_authentication:\n  servers:\n    - endpoint: https://mcp.facebook.com/ads\n      scheme: OAuth 2.0 bearer\n      challenge: >-\n        HTTP 401 with WWW-Authenticate: Bearer resource_metadata=\"https://mcp.facebook.com/.well-known/\n        oauth-protected-resource/ads\", scope=\"ads_management ads_read catalog_management business_management\n        pages_show_list instagram_basic ads_mcp_management\"\n      probed: '2026-08-13'\n    - endpoint: https://mcp.facebook.com/devtools\n      scheme: OAuth 2.0 bearer\n      probed: '2026-08-13'\n  rfc9728: true\n  revocation: facebook.com > Settings > Business Integrations\nauthorization_lifecycle:\n  - name: App Review\n    description: Required before\
  \ an app can use any permission granting access to data it does not own.\n  - name: Business Verification\n    description: Required for all apps requesting Advanced Access.\n  - name: Data Use Checkup\n    description: Annual recertification of permission use.\n  - name: 90-day regrant\n    description: >-\n      A permission unused for 90 days must be granted again by the app user. This revokes working\n      authorization without any API-level warning.\nauthorization_lifecycle_reference: lifecycle/facebook-business-manager-lifecycle.yml\nmutual_tls: false\napi_keys: false\napi_keys_note: >-\n  There is no static API key on this platform. Every call carries an OAuth access token; the closest thing\n  to a long-lived key is a system user token.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/authentication/facebook-business-manager-authentication.yml
summary_line: oauth2/http/openIdConnect · 3 schemes
tags:
- Advertising
- Analytics
- Business Management
- Marketing
- Social-Media
- Messaging
- Commerce
- Agents
- MCP
- Webhook
---
