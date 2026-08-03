---
api_key_in: []
api_specs:
- filename: hyperice-storefront-openapi.yml
  format: yaml
  label: Hyperice Storefront JSON API
  slug: hyperice-storefront-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-storefront-openapi.yml
auth_types:
- none
- openIdConnect
- oauth2
- http
description: 'Hyperice''s authentication profile is not derived from an OpenAPI — it publishes no OpenAPI with securitySchemes. It is read from three live, anonymous discovery documents Hyperice serves on its own domain: the OIDC discovery document, the RFC 8414 OAuth authorization-server metadata (byte-identical to the OIDC document on this store), and the RFC 9728 protected-resource metadata. The result is a three-tier posture: an entirely unauthenticated public read tier, an agent-identity-gated commerce tier, and an OIDC-protected customer-account tier.'
kind: authentication
layout: security
method: probed
name: Hyperice Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hyperice secures its APIs with none, openIdConnect, oauth2, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hyperice
provider_slug: hyperice
scheme_count: 4
schemes:
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
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://accounts.hyperice.com/authentication/logout
  flows:
  - authorizationUrl: https://accounts.hyperice.com/authentication/oauth/authorize
    flow: authorizationCode
    scopes:
      customer-account-api:full: Full access to the Customer Account API on behalf of the buyer.
      customer-account-mcp-api:full: Full access to the Customer Account MCP API on behalf of the buyer.
      email: Release the buyer's email address and email_verified claim.
      openid: Authenticate the buyer and issue an ID token.
    tokenUrl: https://accounts.hyperice.com/authentication/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/78618525910
  jwks_uri: https://accounts.hyperice.com/authentication/.well-known/jwks.json
  name: HypericeCustomerAccounts
  openIdConnectUrl: https://hyperice.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/hyperice-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- authorization_servers:
  - https://accounts.hyperice.com
  - https://shopify.com/authentication/78618525910
  bearer_methods_supported:
  - header
  name: HypericeProtectedResource
  resource: https://hyperice.com
  scheme: bearer
  sources:
  - well-known/hyperice-oauth-protected-resource.json
  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata
  type: http
- description: Non-standard-to-OAuth agent identity gate on the UCP MCP endpoint. The agent must publish a fetchable UCP agent profile document and present its URI; Hyperice's server dereferences it before serving tools.
  name: UCPAgentProfile
  observed_error:
    data_code: invalid_profile_url
    http_status: 422
    jsonrpc_code: -32001
    message: UCP discovery failed
  sources:
  - well-known/hyperice-ucp.json
  - mcp/hyperice-mcp.yml
  type: agent-identity
- description: The Storefront GraphQL API is served in public access mode — no X-Shopify-Storefront-Access-Token is required. An optional Shopify-Storefront-Buyer-IP header is documented in the schema for server-side callers so per-IP throttling attributes to the buyer rather than the caller.
  name: ShopifyStorefrontPublicAccess
  sources:
  - graphql/hyperice-storefront.graphql
  type: none
slug: hyperice-authentication
source_filename: hyperice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://hyperice.com/.well-known/openid-configuration\ndocs: https://hyperice.com/llms.txt\ndescription: >-\n  Hyperice's authentication profile is not derived from an OpenAPI — it publishes\n  no OpenAPI with securitySchemes. It is read from three live, anonymous\n  discovery documents Hyperice serves on its own domain: the OIDC discovery\n  document, the RFC 8414 OAuth authorization-server metadata (byte-identical to\n  the OIDC document on this store), and the RFC 9728 protected-resource\n  metadata. The result is a three-tier posture: an entirely unauthenticated\n  public read tier, an agent-identity-gated commerce tier, and an OIDC-protected\n  customer-account tier.\nsummary:\n  types: [none, openIdConnect, oauth2, http]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  api_key_in: []\n  bearer_methods: [header]\n  unauthenticated_surfaces: 2\ntiers:\n- tier: public-read\n  auth: none\n  surfaces:\n  - https://hyperice.com/products.json\n\
  \  - https://hyperice.com/products/{handle}.json\n  - https://hyperice.com/collections.json\n  - https://hyperice.com/collections/{handle}/products.json\n  - https://hyperice.com/api/2026-04/graphql.json\n  note: >-\n    Verified anonymous on 2026-07-31. Notably the Shopify Storefront GraphQL\n    endpoint answered a FULL introspection query with HTTP 200 and no\n    X-Shopify-Storefront-Access-Token header — this store operates its storefront\n    API in public (unauthenticated) access mode.\n- tier: agentic-commerce\n  auth: ucp-agent-profile\n  surfaces:\n  - https://hyperice.com/api/ucp/mcp\n  note: >-\n    The MCP endpoint requires the calling agent to present a resolvable UCP agent\n    profile URI before it will enumerate or invoke tools. An anonymous\n    tools/list returns HTTP 422, JSON-RPC error -32001 \"UCP discovery failed\",\n    data.code \"invalid_profile_url\". This is an agent-identity gate rather than a\n    bearer-token gate; a bearer token is layered on top for customer-scoped\n\
  \    operations per the protected-resource metadata below.\n- tier: customer-account\n  auth: openIdConnect\n  surfaces:\n  - https://accounts.hyperice.com/\n  note: Buyer sign-in, order history, and the customer-account MCP API.\nschemes:\n- name: HypericeCustomerAccounts\n  type: openIdConnect\n  openIdConnectUrl: https://hyperice.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/78618525910\n  sources: [well-known/hyperice-openid-configuration.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.hyperice.com/authentication/oauth/authorize\n    tokenUrl: https://accounts.hyperice.com/authentication/oauth/token\n    scopes:\n      openid: Authenticate the buyer and issue an ID token.\n      email: Release the buyer's email address and email_verified claim.\n      customer-account-api:full: Full access to the Customer Account API on behalf of the buyer.\n      customer-account-mcp-api:full: Full access to the Customer Account\
  \ MCP API on behalf of the buyer.\n  end_session_endpoint: https://accounts.hyperice.com/authentication/logout\n  jwks_uri: https://accounts.hyperice.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n- name: HypericeProtectedResource\n  type: http\n  scheme: bearer\n  sources: [well-known/hyperice-oauth-protected-resource.json]\n  resource: https://hyperice.com\n  authorization_servers:\n  - https://accounts.hyperice.com\n  - https://shopify.com/authentication/78618525910\n  bearer_methods_supported: [header]\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n- name:\
  \ UCPAgentProfile\n  type: agent-identity\n  sources: [well-known/hyperice-ucp.json, mcp/hyperice-mcp.yml]\n  description: >-\n    Non-standard-to-OAuth agent identity gate on the UCP MCP endpoint. The agent\n    must publish a fetchable UCP agent profile document and present its URI;\n    Hyperice's server dereferences it before serving tools.\n  observed_error:\n    http_status: 422\n    jsonrpc_code: -32001\n    message: UCP discovery failed\n    data_code: invalid_profile_url\n- name: ShopifyStorefrontPublicAccess\n  type: none\n  sources: [graphql/hyperice-storefront.graphql]\n  description: >-\n    The Storefront GraphQL API is served in public access mode — no\n    X-Shopify-Storefront-Access-Token is required. An optional\n    Shopify-Storefront-Buyer-IP header is documented in the schema for\n    server-side callers so per-IP throttling attributes to the buyer rather than\n    the caller.\nnotes:\n- >-\n  There is no API-key surface anywhere on Hyperice's public perimeter — no\n\
  \  apiKey securityScheme, no developer key issuance, no key-management console.\n- >-\n  Hyperice operates no developer program of its own; every authenticated surface\n  is Shopify-operated infrastructure served under Hyperice's own hostnames\n  (hyperice.com, accounts.hyperice.com).\nx-evidence:\n  fetched: '2026-07-31'\n  probes:\n  - {url: 'https://hyperice.com/.well-known/openid-configuration', http_status: 200, content_type: 'application/json'}\n  - {url: 'https://hyperice.com/.well-known/oauth-authorization-server', http_status: 200, content_type: 'application/json'}\n  - {url: 'https://hyperice.com/.well-known/oauth-protected-resource', http_status: 200, content_type: 'application/json'}\n  - {url: 'https://hyperice.com/api/2026-04/graphql.json', method: POST, http_status: 200, authenticated: false, note: 'full introspection, 424 types'}\n  - {url: 'https://hyperice.com/api/ucp/mcp', method: POST, http_status: 422, note: 'invalid_profile_url'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/authentication/hyperice-authentication.yml
summary_line: none/openIdConnect/oauth2/http · 4 schemes
tags:
- Company
- Commerce
- Retail
- Health and Wellness
- Consumer Hardware
- Sports and Fitness
- Agentic Commerce
- GraphQL
- MCP
- Shopify
---
