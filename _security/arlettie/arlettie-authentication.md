---
api_key_in:
- header
auth_types:
- none
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Arlettie Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: Arlettie secures its APIs with none, oauth2, openIdConnect, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: Arlettie
provider_slug: arlettie
scheme_count: 4
schemes:
- applies_to:
  - https://lesechappees.arlettie.com/api/ucp/mcp
  - https://lesechappees.arlettie.com/api/mcp
  - https://lesechappees.arlettie.com/products.json
  - https://lesechappees.arlettie.com/collections.json
  evidence: tools/list returned HTTP 200 with a full tool set and no credential of any kind; the JSON product feeds returned 200 anonymously. No OAuth challenge, no WWW-Authenticate header.
  name: none
  note: Read and cart/checkout construction are anonymous. The gate is not authentication, it is the published human-approval rule on payment completion.
  type: none
- flows:
  - authorizationUrl: https://shopify.com/authentication/86227812661/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token
  - flow: refreshToken
    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token
  issuer: https://shopify.com/authentication/86227812661
  name: shopify-customer-account-oauth
  note: Customer-account authentication for the storefront. The authorization server is Shopify-operated and tenant-scoped to Arlettie's shop id 86227812661; the protected resource it guards is https://lesechappees.arlettie.com. Scopes are catalogued in scopes/arlettie-scopes.yml.
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/arlettie-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  end_session_endpoint: https://shopify.com/authentication/86227812661/logout
  evidence: openid and email are in scopes_supported and an id_token signing algorithm plus a claims set are advertised, so the authorization server is an OIDC provider, not bare OAuth 2.0.
  id_token_signing_alg_values_supported:
  - RS256
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://shopify.com/authentication/86227812661/.well-known/jwks.json
  source: well-known/arlettie-oauth-authorization-server.json
  subject_types_supported:
  - public
  type: openIdConnect
- applies_to:
  - https://lesechappees.arlettie.com/api/2026-04/graphql.json
  documented: false
  in: header
  name: X-Shopify-Storefront-Access-Token
  note: Recorded because the header is the credential an integrator would eventually need for rate-limit-bearing or customer-scoped queries; the anonymous read path above is what actually answers today.
  observed: The Storefront GraphQL endpoint answered a full __schema introspection query and a {shop{name primaryDomain{url} paymentSettings{currencyCode}}} query with HTTP 200 and NO token supplied. Arlettie publishes no token-issuance path and no storefront API documentation, so this header is the platform-standard credential rather than an Arlettie-documented one.
  type: apiKey
slug: arlettie-authentication
source_filename: arlettie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://lesechappees.arlettie.com/.well-known/oauth-authorization-server\nnote: >-\n  Arlettie publishes no OpenAPI, so this profile is not derived from securitySchemes. It is read from\n  the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata served\n  by the Les échappées storefront, plus the observed auth behaviour of each live endpoint.\n\nsummary:\n  types: [none, oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\n  unauthenticated_surfaces: 4\n\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - https://lesechappees.arlettie.com/api/ucp/mcp\n  - https://lesechappees.arlettie.com/api/mcp\n  - https://lesechappees.arlettie.com/products.json\n  - https://lesechappees.arlettie.com/collections.json\n  evidence: >-\n    tools/list returned HTTP 200 with a full tool set and no credential of any kind; the JSON product\n\
  \    feeds returned 200 anonymously. No OAuth challenge, no WWW-Authenticate header.\n  note: >-\n    Read and cart/checkout construction are anonymous. The gate is not authentication, it is the\n    published human-approval rule on payment completion.\n\n- name: shopify-customer-account-oauth\n  type: oauth2\n  source: well-known/arlettie-oauth-authorization-server.json\n  issuer: https://shopify.com/authentication/86227812661\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/86227812661/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token\n    pkce: S256\n  - flow: refreshToken\n    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token\n  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer\n    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token\n  scopes_supported: [openid, email, customer-account-api:full, customer-account-mcp-api:full]\n  token_endpoint_auth_methods_supported:\
  \ [client_secret_basic]\n  note: >-\n    Customer-account authentication for the storefront. The authorization server is Shopify-operated\n    and tenant-scoped to Arlettie's shop id 86227812661; the protected resource it guards is\n    https://lesechappees.arlettie.com. Scopes are catalogued in scopes/arlettie-scopes.yml.\n\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  source: well-known/arlettie-oauth-authorization-server.json\n  openIdConnectUrl: https://shopify.com/authentication/86227812661/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  subject_types_supported: [public]\n  end_session_endpoint: https://shopify.com/authentication/86227812661/logout\n  evidence: >-\n    openid and email are in scopes_supported and an id_token signing algorithm plus a claims set are\n    advertised, so the authorization server is an OIDC provider, not bare OAuth 2.0.\n\n- name:\
  \ shopify-storefront-access-token\n  type: apiKey\n  in: header\n  name: X-Shopify-Storefront-Access-Token\n  applies_to:\n  - https://lesechappees.arlettie.com/api/2026-04/graphql.json\n  documented: false\n  observed: >-\n    The Storefront GraphQL endpoint answered a full __schema introspection query and a\n    {shop{name primaryDomain{url} paymentSettings{currencyCode}}} query with HTTP 200 and NO token\n    supplied. Arlettie publishes no token-issuance path and no storefront API documentation, so this\n    header is the platform-standard credential rather than an Arlettie-documented one.\n  note: >-\n    Recorded because the header is the credential an integrator would eventually need for\n    rate-limit-bearing or customer-scoped queries; the anonymous read path above is what actually\n    answers today.\n\nprotected_resource:\n  source: well-known/arlettie-oauth-protected-resource.json\n  spec: RFC 9728\n  resource: https://lesechappees.arlettie.com\n  authorization_servers: [https://shopify.com/authentication/86227812661]\n\
  \  bearer_methods_supported: [header]\n\nprivate_surfaces:\n- host: api.arlettie.com\n  status: 403\n  note: >-\n    Returns 403 Forbidden on every path including the root. No WWW-Authenticate header is offered, so\n    the auth model is not discoverable — this is an internal service, not a gated public API.\n\nx-evidence:\n  fetched: '2026-08-17'\n  probes:\n  - url: https://lesechappees.arlettie.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://lesechappees.arlettie.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://lesechappees.arlettie.com/api/2026-04/graphql.json\n    http_status: 200\n    note: introspection succeeded with no credential\n  - url: https://lesechappees.arlettie.com/api/ucp/mcp\n    http_status: 200\n    note: tools/list succeeded with no credential\n  - url: https://api.arlettie.com/\n    http_status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arlettie/refs/heads/main/authentication/arlettie-authentication.yml
summary_line: none/oauth2/openIdConnect/apiKey · 4 schemes
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Fashion
- Luxury
- Private Sales
- Marketplace
- Shopify
- Agent Commerce
- MCP
- UCP
---
