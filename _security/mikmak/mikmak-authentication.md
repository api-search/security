---
api_key_in:
- header
api_specs:
- filename: mikmak-authentication-api-openapi.yml
  format: yaml
  label: MikMak Authentication API
  slug: mikmak-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-authentication-api-openapi.yml
- filename: mikmak-availabilities-api-openapi.yml
  format: yaml
  label: MikMak Availabilities API
  slug: mikmak-availabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-availabilities-api-openapi.yml
- filename: mikmak-cart-api-openapi.yml
  format: yaml
  label: MikMak Cart API
  slug: mikmak-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-cart-api-openapi.yml
- filename: mikmak-custom-reports-api-openapi.yml
  format: yaml
  label: MikMak Custom Reports API
  slug: mikmak-custom-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-custom-reports-api-openapi.yml
- filename: mikmak-experiences-api-openapi.yml
  format: yaml
  label: MikMak Experiences API
  slug: mikmak-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-experiences-api-openapi.yml
- filename: mikmak-facet-api-openapi.yml
  format: yaml
  label: MikMak Facet API
  slug: mikmak-facet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-facet-api-openapi.yml
- filename: mikmak-historical-pricing-reports-api-openapi.yml
  format: yaml
  label: MikMak Historical Pricing Reports API
  slug: mikmak-historical-pricing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-historical-pricing-reports-api-openapi.yml
- filename: mikmak-offers-api-openapi.yml
  format: yaml
  label: MikMak Offers API
  slug: mikmak-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-offers-api-openapi.yml
- filename: mikmak-product-api-openapi.yml
  format: yaml
  label: MikMak Product API
  slug: mikmak-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-product-api-openapi.yml
- filename: mikmak-product-search-api-openapi.yml
  format: yaml
  label: MikMak Product Search API
  slug: mikmak-product-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-product-search-api-openapi.yml
- filename: mikmak-shoppable-recipe-reports-api-openapi.yml
  format: yaml
  label: MikMak Shoppable Recipe Reports API
  slug: mikmak-shoppable-recipe-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-shoppable-recipe-reports-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mikmak Authentication
name_suffix: Authentication
oauth_flows: []
overview: MikMak secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MikMak
provider_slug: mikmak
scheme_count: 5
schemes:
- applies_to:
  - MikMak Headless Commerce API
  - MikMak Insights API
  - MikMak Commerce MCP Server
  description: MikMak commerce API key, issued during onboarding. Server-side use only; the docs explicitly warn against exposing it in frontend, mobile or client-side JavaScript.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/mikmak-commerce-api-openapi.yml
  - openapi/mikmak-insights-api-openapi.yml
  - https://docs.mikmak.ai/reference/commerce-api-authentication
  type: apiKey
- applies_to:
  - MikMak Headless Commerce API
  - MikMak Insights API
  - MikMak Commerce MCP Server
  bearerFormat: JWT
  description: 'OAuth 2.0 bearer token presented as `Authorization: Bearer <token>`. Required (not optional) on the hosted MCP endpoint; an alternative to the API key on the Commerce API.'
  name: JWTBearerAuth
  scheme: bearer
  sources:
  - openapi/mikmak-commerce-api-openapi.yml
  - openapi/mikmak-insights-api-openapi.yml
  - https://docs.mikmak.ai/docs/authentication-1
  type: http
- description: Machine-to-machine grant. POST a JSON body of grant_type=client_credentials, client_id and client_secret. Returns access_token, token_type Bearer and expires_in. Token lifetime is configured per application by MikMak, between 24 hours and 30 days. No refresh token is issued for this grant.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  scopes: {}
  sources:
  - https://docs.mikmak.ai/reference/commerce-api-authentication
  tokenUrl: https://api.mikmak.ai/commerce/v1/oauth/token
  type: oauth2
- authorizationUrl: https://api.mikmak.ai/commerce/v1/authorize
  description: User-delegated grant for applications acting on behalf of a logged-in MikMak user (partner dashboards, third-party integrations). redirect_uri must be pre-registered with MikMak. `state` is documented as REQUIRED and must be verified on callback. The authorization code is single-use. Token responses carry expires_in 2592000 (30 days) and a rotating refresh_token — each refresh invalidates the previous refresh token.
  flow: authorizationCode
  name: OAuth2AuthorizationCode
  pkce: not-documented
  refreshUrl: https://api.mikmak.ai/commerce/v1/oauth/token
  scopes:
    offline_access: Issue a refresh token so the application can renew access without user re-consent.
  sources:
  - https://docs.mikmak.ai/reference/authorization-code-flow
  tokenUrl: https://api.mikmak.ai/commerce/v1/oauth/token
  type: oauth2
- description: The hosted MCP server at https://mcp.mikmak.ai/commerce/v1 validates an Auth0-issued JWT. MikMak supplies the token URL, client_id, client_secret and a per-environment `audience` that must be pinned in the token request; a well-formed token minted for the wrong audience is rejected with 401 AUTH_UNAUTHORIZED. Neither the token URL nor the audience is published — both are handed over at onboarding.
  flow: clientCredentials
  name: MCPHostedJWT
  scopes: {}
  sources:
  - https://docs.mikmak.ai/docs/authentication-1
  - https://docs.mikmak.ai/docs/hosted-integration
  token_lifetime_seconds: 86400
  type: oauth2
slug: mikmak-authentication
source_filename: mikmak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.mikmak.ai/reference/commerce-api-authentication\ndocs:\n  - https://docs.mikmak.ai/reference/commerce-api-authentication\n  - https://docs.mikmak.ai/reference/authorization-code-flow\n  - https://docs.mikmak.ai/docs/authentication-1\n  - https://docs.mikmak.ai/docs/mikmak-platform-auth0-enterprise-sso-integration-guide\nderived_from:\n  - openapi/mikmak-commerce-api-openapi.yml\n  - openapi/mikmak-insights-api-openapi.yml\nprovider: MikMak\nproviderId: mikmak\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth_grants:\n    - client_credentials\n    - authorization_code\n    - refresh_token\n  credential_issuance: manual\n  note: >-\n    Credentials are not self-service. MikMak provisions the API key, and one OAuth client\n    (client_id + client_secret) per integrator, during onboarding; there is no public developer\n    signup that issues keys.\nschemes:\n  - name:\
  \ ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >-\n      MikMak commerce API key, issued during onboarding. Server-side use only; the docs\n      explicitly warn against exposing it in frontend, mobile or client-side JavaScript.\n    applies_to:\n      - MikMak Headless Commerce API\n      - MikMak Insights API\n      - MikMak Commerce MCP Server\n    sources:\n      - openapi/mikmak-commerce-api-openapi.yml\n      - openapi/mikmak-insights-api-openapi.yml\n      - https://docs.mikmak.ai/reference/commerce-api-authentication\n  - name: JWTBearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      OAuth 2.0 bearer token presented as `Authorization: Bearer <token>`. Required (not\n      optional) on the hosted MCP endpoint; an alternative to the API key on the Commerce API.\n    applies_to:\n      - MikMak Headless Commerce API\n      - MikMak Insights API\n      - MikMak Commerce MCP Server\n    sources:\n\
  \      - openapi/mikmak-commerce-api-openapi.yml\n      - openapi/mikmak-insights-api-openapi.yml\n      - https://docs.mikmak.ai/docs/authentication-1\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://api.mikmak.ai/commerce/v1/oauth/token\n    description: >-\n      Machine-to-machine grant. POST a JSON body of grant_type=client_credentials, client_id and\n      client_secret. Returns access_token, token_type Bearer and expires_in. Token lifetime is\n      configured per application by MikMak, between 24 hours and 30 days. No refresh token is\n      issued for this grant.\n    scopes: {}\n    sources:\n      - https://docs.mikmak.ai/reference/commerce-api-authentication\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://api.mikmak.ai/commerce/v1/authorize\n    tokenUrl: https://api.mikmak.ai/commerce/v1/oauth/token\n    refreshUrl: https://api.mikmak.ai/commerce/v1/oauth/token\n\
  \    description: >-\n      User-delegated grant for applications acting on behalf of a logged-in MikMak user\n      (partner dashboards, third-party integrations). redirect_uri must be pre-registered with\n      MikMak. `state` is documented as REQUIRED and must be verified on callback. The\n      authorization code is single-use. Token responses carry expires_in 2592000 (30 days) and\n      a rotating refresh_token — each refresh invalidates the previous refresh token.\n    scopes:\n      offline_access: Issue a refresh token so the application can renew access without user re-consent.\n    pkce: not-documented\n    sources:\n      - https://docs.mikmak.ai/reference/authorization-code-flow\n  - name: MCPHostedJWT\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      The hosted MCP server at https://mcp.mikmak.ai/commerce/v1 validates an Auth0-issued JWT.\n      MikMak supplies the token URL, client_id, client_secret and a per-environment `audience`\n      that must\
  \ be pinned in the token request; a well-formed token minted for the wrong\n      audience is rejected with 401 AUTH_UNAUTHORIZED. Neither the token URL nor the audience\n      is published — both are handed over at onboarding.\n    scopes: {}\n    token_lifetime_seconds: 86400\n    sources:\n      - https://docs.mikmak.ai/docs/authentication-1\n      - https://docs.mikmak.ai/docs/hosted-integration\nidentity_headers:\n  - header: x-api-key\n    purpose: MikMak commerce API key. Overrides any server-side configured value.\n  - header: x-wtb-id\n    purpose: WTB (experience) identifier scoping the request to one MikMak experience.\n  - header: X-Request-Id\n    purpose: Optional client-supplied trace id, echoed in MikMak server logs for support correlation.\nresolution_order:\n  order:\n    - value passed on the MCP tool call (wtb_id / api_key arguments)\n    - HTTP request header (x-wtb-id / x-api-key)\n    - server-side configuration on the MCP deployment\n  note: First non-empty value\
  \ wins; a still-missing value returns a configuration error.\nend_user_sso:\n  provider: Auth0\n  protocols:\n    - SAML\n    - OIDC\n  description: >-\n    Enterprise SSO into the MikMak platform (not the API) is brokered through Auth0 against the\n    customer's own IdP.\n  source: https://docs.mikmak.ai/docs/mikmak-platform-auth0-enterprise-sso-integration-guide\ntransport:\n  https_required: true\n  notes:\n    - Tokens and keys must never be sent over non-HTTPS connections.\n    - client_secret must be held in a secret manager and never shipped to a browser.\n    - Rotation of client_secret is requested from MikMak, not self-service.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/authentication/mikmak-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Analytics
- Commerce
- E-Commerce
- Multi-Channel
- Retail Media
- Where to Buy
- Shoppable Media
- Product Availability
- MCP
- agent-native
- Reporting
- CPG
---
