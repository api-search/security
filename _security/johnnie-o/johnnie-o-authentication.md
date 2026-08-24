---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Johnnie O Authentication
name_suffix: Authentication
oauth_flows: []
overview: Johnnie-O declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Johnnie-O
provider_slug: johnnie-o
scheme_count: 4
schemes:
- description: The Hydrogen app proxies the Shopify Storefront API and injects the storefront access token server-side. Anonymous POSTs succeed, including full __schema introspection. No Authorization header, API key or cookie is required by the caller.
  evidence: POST {shop{name}} returned HTTP 200 with data, no credentials sent
  id: storefront-graphql-anonymous
  surface: https://www.johnnie-o.com/api/2024-10/graphql.json
  type: none
  verified: probed
- description: tools/list is anonymous. tools/call requires a UCP agent profile URI; without one every call returns JSON-RPC error -32001 with data.code invalid_profile_url. This is agent identity, not a bearer token or API key.
  evidence: 'POST tools/call search_catalog returned -32001 "Unable to fetch agent profile: Missing profile uri"'
  id: ucp-mcp-agent-profile
  surface: https://checkout.johnnie-o.com/api/ucp/mcp
  type: agent-profile
  verified: probed
- authorization_endpoint: https://shopify.com/authentication/22750137/oauth/authorize
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods:
  - S256
  description: OpenID Connect authorization-code flow with PKCE for Johnnie-O customer accounts. Advertised from checkout.johnnie-o.com/.well-known/openid-configuration and /.well-known/oauth-authorization-server (RFC 8414); the protected resource checkout.johnnie-o.com advertises it via RFC 9728 oauth-protected-resource.
  end_session_endpoint: https://shopify.com/authentication/22750137/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: customer-account-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/22750137
  jwks_uri: https://shopify.com/authentication/22750137/.well-known/jwks.json
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types:
  - public
  surface: https://shopify.com/authentication/22750137
  token_endpoint: https://shopify.com/authentication/22750137/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  verified: probed
- description: Customer-scoped Storefront reads (the customer query, address mutations, order history) take a customerAccessToken minted by the customerAccessTokenCreate mutation and passed as a field argument rather than a header. Anonymous callers can reach the mutation but not another customer's data.
  evidence: 'graphql/johnnie-o-storefront.graphql — QueryRoot.customer(customerAccessToken: String!)'
  id: storefront-customer-access-token
  in: query-argument
  name: customerAccessToken
  surface: https://www.johnnie-o.com/api/2024-10/graphql.json
  type: apiKey
  verified: derived
slug: johnnie-o-authentication
source_filename: johnnie-o-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://checkout.johnnie-o.com/.well-known/openid-configuration + live calls to the\n  storefront GraphQL and UCP MCP endpoints\nnote: >-\n  Three distinct auth postures coexist on Johnnie-O's surfaces, and they are not the same\n  story. The identity provider is Shopify's per-merchant customer-accounts issuer for shop\n  22750137; Johnnie-O did not author it, but it is advertised from Johnnie-O's own primary\n  domain and issues tokens for Johnnie-O's customers.\nschemes:\n- id: storefront-graphql-anonymous\n  surface: https://www.johnnie-o.com/api/2024-10/graphql.json\n  type: none\n  description: >-\n    The Hydrogen app proxies the Shopify Storefront API and injects the storefront access\n    token server-side. Anonymous POSTs succeed, including full __schema introspection. No\n    Authorization header, API key or cookie is required by the caller.\n  verified: probed\n  evidence: 'POST {shop{name}} returned HTTP 200 with\
  \ data, no credentials sent'\n- id: ucp-mcp-agent-profile\n  surface: https://checkout.johnnie-o.com/api/ucp/mcp\n  type: agent-profile\n  description: >-\n    tools/list is anonymous. tools/call requires a UCP agent profile URI; without one every\n    call returns JSON-RPC error -32001 with data.code invalid_profile_url. This is agent\n    identity, not a bearer token or API key.\n  verified: probed\n  evidence: 'POST tools/call search_catalog returned -32001 \"Unable to fetch agent profile:\n    Missing profile uri\"'\n- id: customer-account-oidc\n  surface: https://shopify.com/authentication/22750137\n  type: openIdConnect\n  description: >-\n    OpenID Connect authorization-code flow with PKCE for Johnnie-O customer accounts.\n    Advertised from checkout.johnnie-o.com/.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server (RFC 8414); the protected resource\n    checkout.johnnie-o.com advertises it via RFC 9728 oauth-protected-resource.\n  verified: probed\n\
  \  issuer: https://shopify.com/authentication/22750137\n  authorization_endpoint: https://shopify.com/authentication/22750137/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/22750137/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/22750137/logout\n  jwks_uri: https://shopify.com/authentication/22750137/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  subject_types: [public]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n- id: storefront-customer-access-token\n  surface: https://www.johnnie-o.com/api/2024-10/graphql.json\n  type: apiKey\n  in: query-argument\n  name: customerAccessToken\n  description:\
  \ >-\n    Customer-scoped Storefront reads (the customer query, address mutations, order history)\n    take a customerAccessToken minted by the customerAccessTokenCreate mutation and passed as\n    a field argument rather than a header. Anonymous callers can reach the mutation but not\n    another customer's data.\n  verified: derived\n  evidence: \"graphql/johnnie-o-storefront.graphql \\u2014 QueryRoot.customer(customerAccessToken: String!)\"\nprotected_resources:\n- resource: https://checkout.johnnie-o.com\n  authorization_servers: [https://shopify.com/authentication/22750137]\n  bearer_methods_supported: [header]\n  rfc: RFC 9728\nmtls: false\napi_keys_public: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnnie-o/refs/heads/main/authentication/johnnie-o-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Apparel
- Retail
- E-Commerce
- Direct to Consumer
- Golf
- Fashion
- Consumer Goods
- Shopify
- Agentic Commerce
---
