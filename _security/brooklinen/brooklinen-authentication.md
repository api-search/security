---
api_key_in: []
api_specs:
- filename: brooklinen-cart-api-openapi.yml
  format: yaml
  label: Brooklinen Cart API
  slug: brooklinen-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-cart-api-openapi.yml
- filename: brooklinen-collections-api-openapi.yml
  format: yaml
  label: Brooklinen Collections API
  slug: brooklinen-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-collections-api-openapi.yml
- filename: brooklinen-discovery-api-openapi.yml
  format: yaml
  label: Brooklinen Discovery API
  slug: brooklinen-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-discovery-api-openapi.yml
- filename: brooklinen-products-api-openapi.yml
  format: yaml
  label: Brooklinen Products API
  slug: brooklinen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-products-api-openapi.yml
- filename: brooklinen-search-api-openapi.yml
  format: yaml
  label: Brooklinen Search API
  slug: brooklinen-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-search-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- none
description: ''
kind: authentication
layout: security
method: probed
name: Brooklinen Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Brooklinen secures its APIs with oauth2, openIdConnect, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Brooklinen
provider_slug: brooklinen
scheme_count: 4
schemes:
- applies_to: openapi/brooklinen-storefront-openapi.yml
  description: The documented read-only storefront JSON endpoints (/products.json, /products/{handle}.json, /collections/{handle}/products.json, /search/suggest.json, /cart.js) require no credential. Confirmed by anonymous HTTP 200 on each, 2026-08-02.
  name: none
  type: none
- applies_to: https://www.brooklinen.com/api/ucp/mcp
  description: The MCP endpoint requires the calling agent to identify itself with a URI pointing at its own UCP profile document, which the merchant fetches. This is agent identity, not user authorization — it gates tools/list as well as tool invocation. An anonymous or unresolvable profile returns HTTP 422 with JSON-RPC error -32001 (`invalid_profile_url`).
  in: header
  name: ucp-agent-profile
  parameter_name: UCP-Agent
  request_property: meta.ucp-agent.profile
  required: true
  sources:
  - https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json
  type: agentIdentity
- applies_to: https://www.brooklinen.com
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.0 authorization code flow with PKCE against Shopify's customer account issuer for this shop, fronted on Brooklinen's own account subdomain. Covers customer account data and the customer account MCP API.
  end_session_endpoint: https://account.brooklinen.com/authentication/logout
  flows:
  - authorizationUrl: https://account.brooklinen.com/authentication/oauth/authorize
    flow: authorizationCode
    scopes:
      customer-account-api:full: Full access to the Shopify Customer Account API for this shop.
      customer-account-mcp-api:full: Full access to the Customer Account MCP API for this shop.
      email: Access to the customer's email address.
      openid: OpenID Connect authentication.
    tokenUrl: https://account.brooklinen.com/authentication/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/9517126
  name: shopify-customer-account-oauth2
  sources:
  - https://www.brooklinen.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
- applies_to: https://www.brooklinen.com
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
  description: The same issuer advertises OpenID Connect metadata — JWKS, RS256 id_token signing, and standard claims — though no /.well-known/openid-configuration is served at the store origin.
  id_token_signing_alg_values_supported:
  - RS256
  jwks_uri: https://account.brooklinen.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oidc
  response_types_supported:
  - code
  sources:
  - https://www.brooklinen.com/.well-known/oauth-authorization-server
  subject_types_supported:
  - public
  type: openIdConnect
slug: brooklinen-authentication
source_filename: brooklinen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource:\n- https://www.brooklinen.com/.well-known/oauth-authorization-server\n- https://www.brooklinen.com/.well-known/oauth-protected-resource\n- https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json\nsummary:\n  types: [oauth2, openIdConnect, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  bearer: header\n  note: >-\n    Brooklinen runs no developer API key program. Two distinct authentication postures exist: the read-only\n    storefront JSON surface is fully anonymous, and the transactional UCP/MCP surface is gated by agent\n    identity (a resolvable UCP agent profile) with customer authorization handled by Shopify's OAuth 2.0 /\n    OIDC customer account issuer.\nschemes:\n- name: none\n  type: none\n  applies_to: openapi/brooklinen-storefront-openapi.yml\n  description: >-\n    The documented read-only storefront JSON endpoints (/products.json, /products/{handle}.json,\n    /collections/{handle}/products.json,\
  \ /search/suggest.json, /cart.js) require no credential. Confirmed by\n    anonymous HTTP 200 on each, 2026-08-02.\n- name: ucp-agent-profile\n  type: agentIdentity\n  in: header\n  parameter_name: UCP-Agent\n  request_property: meta.ucp-agent.profile\n  required: true\n  applies_to: https://www.brooklinen.com/api/ucp/mcp\n  description: >-\n    The MCP endpoint requires the calling agent to identify itself with a URI pointing at its own UCP profile\n    document, which the merchant fetches. This is agent identity, not user authorization — it gates\n    tools/list as well as tool invocation. An anonymous or unresolvable profile returns HTTP 422 with\n    JSON-RPC error -32001 (`invalid_profile_url`).\n  sources: [https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json]\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  applies_to: https://www.brooklinen.com\n  description: >-\n    OAuth 2.0 authorization code flow with PKCE against Shopify's customer account issuer for this\
  \ shop,\n    fronted on Brooklinen's own account subdomain. Covers customer account data and the customer account MCP\n    API.\n  issuer: https://shopify.com/authentication/9517126\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.brooklinen.com/authentication/oauth/authorize\n    tokenUrl: https://account.brooklinen.com/authentication/oauth/token\n    scopes:\n      openid: OpenID Connect authentication.\n      email: Access to the customer's email address.\n      customer-account-api:full: Full access to the Shopify Customer Account API for this shop.\n      customer-account-mcp-api:full: Full access to the Customer Account MCP API for this shop.\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  end_session_endpoint: https://account.brooklinen.com/authentication/logout\n  sources: [https://www.brooklinen.com/.well-known/oauth-authorization-server]\n\
  - name: shopify-customer-account-oidc\n  type: openIdConnect\n  applies_to: https://www.brooklinen.com\n  description: >-\n    The same issuer advertises OpenID Connect metadata — JWKS, RS256 id_token signing, and standard claims —\n    though no /.well-known/openid-configuration is served at the store origin.\n  jwks_uri: https://account.brooklinen.com/authentication/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  response_types_supported: [code]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources: [https://www.brooklinen.com/.well-known/oauth-authorization-server]\nprotected_resource:\n  resource: https://www.brooklinen.com\n  authorization_servers:\n  - https://account.brooklinen.com\n  - https://shopify.com/authentication/9517126\n  bearer_methods_supported: [header]\n  spec: RFC 9728\n  sources: [https://www.brooklinen.com/.well-known/oauth-protected-resource]\nhuman_in_the_loop:\n\
  \  required_for: [complete_checkout]\n  policy: >-\n    Brooklinen's /agents.md and /robots.txt both state that checkout, payment and order placement must not be\n    completed automatically. Agents must obtain explicit, contemporaneous human approval at the moment of\n    payment, or route the purchase through Shop Pay via https://shop.app/SKILL.md.\nx-evidence:\n  fetched: '2026-08-02'\n  probes:\n  - {url: 'https://www.brooklinen.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://www.brooklinen.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://www.brooklinen.com/.well-known/openid-configuration', http_status: 404}\n  - {url: 'https://www.brooklinen.com/products.json?limit=1', http_status: 200, auth: none}\n  - {url: 'https://www.brooklinen.com/api/ucp/mcp', http_status: 422, auth: none}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/authentication/brooklinen-authentication.yml
summary_line: oauth2/openIdConnect/none · 4 schemes
tags:
- ecommerce
- retail
- direct-to-consumer
- home-goods
- bedding
- shopify
- agentic-commerce
- universal-commerce-protocol
- mcp
- agent-native
- catalog
- checkout
---
