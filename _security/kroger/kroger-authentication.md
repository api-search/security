---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Kroger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kroger declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kroger
provider_slug: kroger
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization server operated by Kroger at api.kroger.com. Three grant types are documented.
  flows:
    authorizationCode:
      authorizationUrl: https://api.kroger.com/v1/connect/oauth2/authorize
      client_authentication: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'
      parameters:
        client_id: registered application client id
        redirect_uri: must exactly match a redirect URL registered for the app
        response_type: code
        scope: space-delimited list of registered scopes
      pkce: Documented as available — the portal's Postman guide instructs "Authorization Code (with PKCE)". Not stated as mandatory.
      tokenUrl: https://api.kroger.com/v1/connect/oauth2/token
      use_when: The application acts on behalf of an authenticated Kroger customer (Identity, Cart).
    clientCredentials:
      client_authentication: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'
      parameters:
        grant_type: client_credentials
        scope: space-delimited list of registered scopes
      request_content_type: application/x-www-form-urlencoded
      tokenUrl: https://api.kroger.com/v1/connect/oauth2/token
      use_when: The application requests general data or data owned by the application (Products, Locations).
    refreshToken:
      note: Refresh tokens are only issued by the Authorization Code grant. A refresh returns BOTH a new access token and a new refresh token, and the old refresh token becomes invalid once used (single-use rotation).
      parameters:
        grant_type: refresh_token
        refresh_token: the refresh token issued with the original access token
      tokenUrl: https://api.kroger.com/v1/connect/oauth2/token
  id: kroger_oauth2
  type: oauth2
slug: kroger-authentication
source_filename: kroger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Kroger\nproviderId: kroger\ngenerated: '2026-08-27'\nmethod: searched\nsource: >-\n  Kroger developer documentation, read anonymously from the portal's own content\n  API (https://developer.kroger.com/api/v1/developer/content/search.json, HTTP\n  200) because developer.kroger.com renders every page client-side.\ndocs:\n  - https://developer.kroger.com/documentation/public/security/guides-oauth\n  - https://developer.kroger.com/documentation/public/security/service-to-service\n  - https://developer.kroger.com/documentation/public/security/customer\n  - https://developer.kroger.com/documentation/public/security/refresh-token-tutorial\n  - https://developer.kroger.com/documentation/public/getting-started/quick-start\nsummary: >-\n  Every Kroger Public and Partner API is protected by OAuth 2.0. There is no API\n  key, no basic-auth-to-the-resource and no mTLS surface. Applications register\n  on the\
  \ developer portal for a client_id/client_secret pair, exchange them at a\n  single token endpoint, and present a bearer access token to the resource\n  server. Scopes are assigned to the application at registration time and cannot\n  be self-expanded at runtime.\nschemes:\n  - id: kroger_oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization server operated by Kroger at api.kroger.com. Three\n      grant types are documented.\n    flows:\n      clientCredentials:\n        tokenUrl: https://api.kroger.com/v1/connect/oauth2/token\n        client_authentication: >-\n          HTTP Basic — Authorization: Basic base64(client_id:client_secret)\n        request_content_type: application/x-www-form-urlencoded\n        parameters:\n          grant_type: client_credentials\n          scope: space-delimited list of registered scopes\n        use_when: >-\n          The application requests general data or data owned by the application\n          (Products, Locations).\n   \
  \   authorizationCode:\n        authorizationUrl: https://api.kroger.com/v1/connect/oauth2/authorize\n        tokenUrl: https://api.kroger.com/v1/connect/oauth2/token\n        client_authentication: >-\n          HTTP Basic — Authorization: Basic base64(client_id:client_secret)\n        parameters:\n          response_type: code\n          client_id: registered application client id\n          redirect_uri: must exactly match a redirect URL registered for the app\n          scope: space-delimited list of registered scopes\n        pkce: >-\n          Documented as available — the portal's Postman guide instructs\n          \"Authorization Code (with PKCE)\". Not stated as mandatory.\n        use_when: >-\n          The application acts on behalf of an authenticated Kroger customer\n          (Identity, Cart).\n      refreshToken:\n        tokenUrl: https://api.kroger.com/v1/connect/oauth2/token\n        parameters:\n          grant_type: refresh_token\n          refresh_token: the refresh\
  \ token issued with the original access token\n        note: >-\n          Refresh tokens are only issued by the Authorization Code grant. A\n          refresh returns BOTH a new access token and a new refresh token, and\n          the old refresh token becomes invalid once used (single-use rotation).\nresource_authorization:\n  header: 'Authorization: Bearer {access_token}'\n  applies_to: all Public and Partner API endpoints\ntoken:\n  access_token:\n    type: bearer\n    format: JWT (RS256; iss api.kroger.com, carries scope, aud, sub, exp, iat)\n    lifetime_seconds: 1800\n    lifetime_note: 'Documented as \"Access tokens expire every thirty minutes\"; expires_in returns 1800.'\n  refresh_token:\n    lifetime: six months\n    rotation: single-use — invalid once redeemed\nconsent:\n  customer_consent_required: true\n  description: >-\n    Under the Authorization Code grant the customer signs in at Kroger and is\n    shown the specific scopes the application is requesting before granting.\
  \ The\n    token carries both the scope set and the customer's consent.\n  denial_behavior: >-\n    error=access_denied&error_description=The+resource+owner+denied+the+request\n    is appended to the registered redirect URL.\nerrors:\n  unauthenticated:\n    status: 401\n    body: '{\"error\":\"invalid_request\",\"error_description\":\"The access_token is missing\"}'\n    observed: 'Live probe of https://api.kroger.com/v1/products, 2026-08-27, HTTP 401.'\n  expired_token:\n    status: 401\n    body: '{\"error\":\"invalid_token\",\"error_description\":\"The access token is invalid or has expired\"}'\n  missing_scope:\n    status: 403\n    body: '{\"errors\":{\"timestamp\":1567098508093,\"code\":\"Forbidden\",\"reason\":\"missing required scopes\"}}'\nnot_supported:\n  - openIdConnect — no /.well-known/openid-configuration on any Kroger host (404)\n  - oauth-authorization-server metadata (RFC 8414) — 404 on api.kroger.com and api-ce.kroger.com\n  - oauth-protected-resource metadata (RFC\
  \ 9728) — 404 on api.kroger.com\n  - dynamic client registration (RFC 7591) — registration is a human form on the developer portal\n  - apiKey, mutualTLS, http basic against the resource server\nonboarding:\n  public_apis: >-\n    Self-service. Create an account on developer.kroger.com, verify by email,\n    register an application, receive client_id/client_secret.\n  partner_apis: >-\n    Not self-service. Requires a submitted Partner Request and a contractual\n    agreement with Kroger.\n  scope_changes: >-\n    Scopes are assigned during app registration and can only be changed by\n    request to Kroger; an application cannot request a scope it was not granted.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kroger/refs/heads/main/authentication/kroger-authentication.yml
summary_line: 1 scheme
tags:
- Groceries
- Grocery Retail
- Retail
- Ecommerce
- Product Catalog
- Store Locations
- Shopping Cart
- Loyalty
- OAuth
- Partner API
- Fortune 100
---
