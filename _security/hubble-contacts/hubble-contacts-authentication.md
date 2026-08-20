---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
- none
description: ''
kind: authentication
layout: security
method: searched
name: Hubble Contacts Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hubble Contacts secures its APIs with oauth2, openIdConnect, http, and none across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hubble Contacts
provider_slug: hubble-contacts
scheme_count: 2
schemes:
- applies_to: Customer account access (order history, subscription management)
  authorization_endpoint: https://shopify.com/authentication/15165228/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/15165228/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/15165228
  jwks_uri: https://shopify.com/authentication/15165228/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://account.hubblecontacts.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/hubble-contacts-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/15165228/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/15165228/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/15165228/oauth/token
  issuer: https://shopify.com/authentication/15165228
  metadata: https://account.hubblecontacts.com/.well-known/oauth-authorization-server
  name: shopify-oauth-authorization-server
  source: well-known/hubble-contacts-oauth-authorization-server.json
  standard: RFC 8414
  type: oauth2
slug: hubble-contacts-authentication
source_filename: hubble-contacts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://account.hubblecontacts.com/.well-known/openid-configuration\ndocs: https://account.hubblecontacts.com/agents.md\nnotes: >-\n  Hubble Contacts publishes no OpenAPI, so this profile is not derived from\n  securitySchemes — it is read directly from the OAuth 2.0 / OpenID Connect discovery\n  documents the storefront host serves, plus the observed auth behaviour of the two\n  public surfaces. The authorization server is the Shopify customer accounts issuer\n  bound to Hubble's shop id 15165228; the protected resource is Hubble's own host.\nsummary:\n  types: [oauth2, openIdConnect, http, none]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  bearer_methods: [header]\n  api_key_in: []\nschemes:\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://account.hubblecontacts.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/15165228\n  authorization_endpoint:\
  \ https://shopify.com/authentication/15165228/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/15165228/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/15165228/logout\n  jwks_uri: https://shopify.com/authentication/15165228/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes_supported:\n  - openid\n  - email\n  - 'customer-account-api:full'\n  - 'customer-account-mcp-api:full'\n  applies_to: Customer account access (order history, subscription management)\n  source: well-known/hubble-contacts-openid-configuration.json\n- name: shopify-oauth-authorization-server\n\
  \  type: oauth2\n  metadata: https://account.hubblecontacts.com/.well-known/oauth-authorization-server\n  standard: RFC 8414\n  issuer: https://shopify.com/authentication/15165228\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/15165228/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/15165228/oauth/token\n    pkce: S256\n  source: well-known/hubble-contacts-oauth-authorization-server.json\nprotected_resources:\n- resource: https://account.hubblecontacts.com\n  standard: RFC 9728\n  metadata: https://account.hubblecontacts.com/.well-known/oauth-protected-resource\n  authorization_servers: ['https://shopify.com/authentication/15165228']\n  bearer_methods_supported: [header]\n  source: well-known/hubble-contacts-oauth-protected-resource.json\n- name: shopify-storefront-customer-access-token\n  type: http\n  scheme: bearer-like custom token\n  surface: Storefront GraphQL\n  issued_by: 'mutation customerAccessTokenCreate(input:\
  \ {email, password})'\n  renewed_by: customerAccessTokenRenew\n  revoked_by: customerAccessTokenDelete\n  passed_as: 'customerAccessToken argument on customer-scoped fields and cart mutations'\n  applies_to: 'Customer-scoped reads/writes on the Storefront GraphQL surface (customer profile, addresses, orders)'\n  source: graphql/hubble-contacts-storefront.graphql\n  note: >-\n    Found in round 2. Distinct from the OIDC customer-accounts issuer above: this is\n    the legacy Storefront-API token exchange, which Shopify is steering to the\n    Customer Account API. Anonymous callers reach everything else on the surface.\nsurfaces:\n- surface: Storefront GraphQL\n  base: 'https://account.hubblecontacts.com/api/{version}/graphql.json'\n  auth: none\n  observed: >-\n    Round 2. POST with no X-Shopify-Storefront-Access-Token and no bearer token\n    returned HTTP 200 for a full introspection query (416 types) and for real data\n    queries (shop { name } returned \"Hubble Contacts\"). The server\
  \ labelled the call\n    graphql;desc=\"storefront/query/anonymous\". Only customer-scoped fields require a\n    customerAccessToken. This is the most open surface on the property and it is\n    documented nowhere by Hubble.\n- surface: Storefront Product JSON\n  base: https://account.hubblecontacts.com\n  auth: none\n  observed: >-\n    GET /products.json, /products/{handle}.json, /collections/{handle}/products.json\n    and /search all return HTTP 200 with no credentials.\n- surface: UCP Commerce MCP\n  base: https://account.hubblecontacts.com/api/ucp/mcp\n  auth: ucp-agent-profile\n  observed: >-\n    Anonymous JSON-RPC returns HTTP 422 / -32001 invalid_profile_url. The gate is a\n    registered UCP agent profile URI rather than an OAuth bearer challenge; no\n    WWW-Authenticate header was returned. Buyer-side payment is separately gated on\n    explicit human approval per Hubble's /agents.md.\n- surface: Marketing site\n  base: https://www.hubblecontacts.com\n  auth: none\n  observed:\
  \ No auth-bearing API surface; no /.well-known/ documents served.\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - {url: 'https://account.hubblecontacts.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://account.hubblecontacts.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://account.hubblecontacts.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://account.hubblecontacts.com/api/ucp/mcp', method: POST, http_status: 422}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubble-contacts/refs/heads/main/authentication/hubble-contacts-authentication.yml
summary_line: oauth2/openIdConnect/http/none · 2 schemes
tags:
- Company
- E-Commerce
- Retail
- Health
- Vision Care
- Contact Lenses
- Subscription
- Agentic Commerce
- MCP
- Shopify
- GraphQL
---
