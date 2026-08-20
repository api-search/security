---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- none
description: ''
kind: authentication
layout: security
method: probed
name: Athletic Greens Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- refresh_token
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: AG1 secures its APIs with oauth2, openIdConnect, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, refresh_token, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: AG1
provider_slug: athletic-greens
scheme_count: 4
schemes:
- authorization_endpoint: https://account.drinkag1.com/authentication/oauth/authorize
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
  end_session_endpoint: https://account.drinkag1.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/15234600
  jwks_uri: https://account.drinkag1.com/authentication/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://account.drinkag1.com/.well-known/openid-configuration
  protects:
  - https://account.drinkag1.com/customer/api/mcp
  - https://shop.drinkag1.com (declared resource in /.well-known/oauth-protected-resource)
  response_types_supported:
  - code
  scopes: scopes/athletic-greens-scopes.yml
  sources:
  - well-known/athletic-greens-oauth-authorization-server.json
  - well-known/athletic-greens-openid-configuration.json
  - well-known/athletic-greens-jwks.json
  subject_types_supported:
  - public
  token_endpoint: https://account.drinkag1.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- applies_to: https://shop.drinkag1.com/api/mcp
  name: storefront-mcp-anonymous
  observed: JSON-RPC tools/list and catalog/cart tools answered 200 with no credential on 2026-08-02
  type: none
- applies_to: https://shop.drinkag1.com/api/{version}/graphql.json
  name: storefront-graphql-public
  observed: full anonymous introspection succeeded; the public storefront token is injected by the storefront edge rather than required from the caller
  type: none
- applies_to: https://shop.drinkag1.com/api/ucp/mcp
  name: ucp-agent-profile
  observed: 'anonymous tools/list returned HTTP 422 with JSON-RPC -32001 invalid_profile_url ("Unable to fetch agent profile: Missing profile uri"); the UCP transport authenticates the calling agent by a resolvable agent profile URI passed in meta.ucp-agent.profile'
  type: agent-profile
slug: athletic-greens-authentication
source_filename: athletic-greens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://shop.drinkag1.com/.well-known/oauth-authorization-server\ndocs: https://shop.drinkag1.com/agents.md\nnote: AG1 publishes no OpenAPI, so this profile is built from live RFC 8414 / OIDC\n  discovery documents and from observed behaviour of each surface, not from\n  securitySchemes.\nsummary:\n  types: [oauth2, openIdConnect, none]\n  api_key_in: []\n  oauth2_flows: [authorization_code, refresh_token, urn:ietf:params:oauth:grant-type:jwt-bearer]\n  pkce: S256\n  bearer_methods: [header]\nschemes:\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://account.drinkag1.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/15234600\n  authorization_endpoint: https://account.drinkag1.com/authentication/oauth/authorize\n  token_endpoint: https://account.drinkag1.com/authentication/oauth/token\n  end_session_endpoint: https://account.drinkag1.com/authentication/logout\n\
  \  jwks_uri: https://account.drinkag1.com/authentication/.well-known/jwks.json\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: scopes/athletic-greens-scopes.yml\n  protects:\n  - https://account.drinkag1.com/customer/api/mcp\n  - https://shop.drinkag1.com (declared resource in /.well-known/oauth-protected-resource)\n  sources:\n  - well-known/athletic-greens-oauth-authorization-server.json\n  - well-known/athletic-greens-openid-configuration.json\n  - well-known/athletic-greens-jwks.json\n- name: storefront-mcp-anonymous\n  type: none\n  applies_to: https://shop.drinkag1.com/api/mcp\n  observed: 'JSON-RPC tools/list\
  \ and catalog/cart tools answered 200 with no credential\n    on 2026-08-02'\n- name: storefront-graphql-public\n  type: none\n  applies_to: https://shop.drinkag1.com/api/{version}/graphql.json\n  observed: full anonymous introspection succeeded; the public storefront token is\n    injected by the storefront edge rather than required from the caller\n- name: ucp-agent-profile\n  type: agent-profile\n  applies_to: https://shop.drinkag1.com/api/ucp/mcp\n  observed: 'anonymous tools/list returned HTTP 422 with JSON-RPC -32001\n    invalid_profile_url (\"Unable to fetch agent profile: Missing profile uri\"); the\n    UCP transport authenticates the calling agent by a resolvable agent profile URI\n    passed in meta.ucp-agent.profile'\nprotected_resources:\n- resource: https://shop.drinkag1.com\n  authorization_servers: [https://account.drinkag1.com, https://shopify.com/authentication/15234600]\n  bearer_methods_supported: [header]\n  source: well-known/athletic-greens-oauth-protected-resource.json\n\
  - resource: https://account.drinkag1.com\n  authorization_servers: [https://account.drinkag1.com, https://shopify.com/authentication/15234600]\n  bearer_methods_supported: [header]\n  source: well-known/athletic-greens-account-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athletic-greens/refs/heads/main/authentication/athletic-greens-authentication.yml
summary_line: oauth2/openIdConnect/none · 4 schemes
tags:
- Company
- Consumer
- Health
- Nutrition
- Supplements
- Direct to Consumer
- E-Commerce
- Subscription
- Wellness
- Agentic Commerce
- MCP
- UCP
- Shopify
- GraphQL
---
