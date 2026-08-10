---
api_key_in: []
auth_types: []
description: Authentication profile for the Athletic Brewing storefront's agent and customer surfaces. Derived entirely from documents the host serves anonymously — the OpenID Connect discovery document, the RFC 8414 authorization-server metadata, the RFC 9728 protected-resource metadata, and live introspection of the UCP/MCP endpoint. Nothing here is inferred from a private or credentialed source.
kind: authentication
layout: security
method: probed
name: Athletic Brewing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Athletic Brewing declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Athletic Brewing
provider_slug: athletic-brewing
scheme_count: 3
schemes:
- authorization_endpoint: https://shopify.com/authentication/7931756625/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/7931756625/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/7931756625
  jwks_uri: https://shopify.com/authentication/7931756625/.well-known/jwks.json
  notes: PKCE with S256 is the only code_challenge_method offered. The authorization server is operated by Shopify on behalf of the merchant; the discovery document is served from Athletic Brewing's own domain.
  openIdConnectUrl: https://athleticbrewing.com/.well-known/openid-configuration
  pkce_required: true
  response_types_supported:
  - code
  scopes: scopes/athletic-brewing-scopes.yml
  subject_types_supported:
  - public
  surface: customer accounts / buyer-scoped commerce
  token_endpoint: https://shopify.com/authentication/7931756625/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- authorization_servers:
  - https://shopify.com/authentication/7931756625
  bearer_methods_supported:
  - header
  id: ucp-protected-resource
  resource: https://athleticbrewing.com
  scheme: bearer
  source: https://athleticbrewing.com/.well-known/oauth-protected-resource
  spec: RFC 9728
  surface: athleticbrewing.com as an OAuth protected resource
  type: http
- anonymous_operations:
  - initialize
  - tools/list
  failure_mode:
    data_code: invalid_profile_url
    http_status: 422
    jsonrpc_error_code: -32001
    message: UCP discovery failed
  id: ucp-agent-profile
  mechanism: Every tools/call must carry meta.ucp-agent.profile, a resolvable URI identifying the calling agent, which the server fetches. This is agent identity, not buyer authorization — it gates who may call, not what a buyer has consented to.
  surface: UCP/MCP endpoint (https://athleticbrewing.com/api/ucp/mcp)
  type: other
slug: athletic-brewing-authentication
source_filename: athletic-brewing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://athleticbrewing.com/.well-known/openid-configuration\ndocs: https://athleticbrewing.com/agents.md\ndescription: >-\n  Authentication profile for the Athletic Brewing storefront's agent and customer surfaces.\n  Derived entirely from documents the host serves anonymously — the OpenID Connect discovery\n  document, the RFC 8414 authorization-server metadata, the RFC 9728 protected-resource\n  metadata, and live introspection of the UCP/MCP endpoint. Nothing here is inferred from\n  a private or credentialed source.\nschemes:\n- id: shopify-customer-accounts-oidc\n  type: openIdConnect\n  surface: customer accounts / buyer-scoped commerce\n  openIdConnectUrl: https://athleticbrewing.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/7931756625\n  authorization_endpoint: https://shopify.com/authentication/7931756625/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/7931756625/oauth/token\n\
  \  end_session_endpoint: https://shopify.com/authentication/7931756625/logout\n  jwks_uri: https://shopify.com/authentication/7931756625/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: scopes/athletic-brewing-scopes.yml\n  pkce_required: true\n  notes: >-\n    PKCE with S256 is the only code_challenge_method offered. The authorization server is\n    operated by Shopify on behalf of the merchant; the discovery document is served from\n    Athletic Brewing's own domain.\n- id: ucp-protected-resource\n  type: http\n  scheme: bearer\n  surface: athleticbrewing.com as an OAuth protected\
  \ resource\n  source: https://athleticbrewing.com/.well-known/oauth-protected-resource\n  resource: https://athleticbrewing.com\n  authorization_servers:\n  - https://shopify.com/authentication/7931756625\n  bearer_methods_supported: [header]\n  spec: RFC 9728\n- id: ucp-agent-profile\n  type: other\n  surface: UCP/MCP endpoint (https://athleticbrewing.com/api/ucp/mcp)\n  mechanism: >-\n    Every tools/call must carry meta.ucp-agent.profile, a resolvable URI identifying the\n    calling agent, which the server fetches. This is agent identity, not buyer\n    authorization — it gates who may call, not what a buyer has consented to.\n  anonymous_operations:\n  - initialize\n  - tools/list\n  failure_mode:\n    http_status: 422\n    jsonrpc_error_code: -32001\n    message: UCP discovery failed\n    data_code: invalid_profile_url\nanonymous_access:\n  tools_list: true\n  catalog_json: true\n  note: >-\n    Product and collection JSON (/products.json, /collections/{handle}/products.json) and\n\
  \    MCP tools/list are readable with no credentials at all.\nconsent:\n  payment_requires_human_approval: true\n  source: https://athleticbrewing.com/llms.txt\n  statement: >-\n    \"Checkout requires human approval. Agents must not complete payment without explicit\n    buyer consent.\" Restated in robots.txt.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://athleticbrewing.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://athleticbrewing.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://athleticbrewing.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://athleticbrewing.com/api/ucp/mcp\n    http_status: 422\n    note: tools/call without meta.ucp-agent.profile\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athletic-brewing/refs/heads/main/authentication/athletic-brewing-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Non-Alcoholic Beer
- Beverage
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
