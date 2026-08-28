---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Prime Hydration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prime Hydration declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Prime Hydration
provider_slug: prime-hydration
scheme_count: 3
schemes:
- applies_to: https://drinkprime.com/api/ucp/mcp
  description: The UCP shopping MCP endpoint answers tools/list anonymously - no Authorization header, no API key, no OAuth challenge. Catalog search/lookup, cart and checkout construction are all reachable without credentials.
  evidence: POST /api/ucp/mcp with no Authorization header returned HTTP 200 and the full 13-tool manifest with inputSchemas.
  id: none
  identity_substitute: 'Instead of a credential, every tool requires meta.ucp-agent.profile - a URI identifying the calling agent. This is agent attestation/discovery, not authentication: it is unverified caller-asserted metadata and grants no privilege.'
  type: none
- applies_to: complete_checkout
  description: Payment is authorized by the human buyer, not by the agent. complete_checkout additionally requires meta.idempotency-key. Buyer approval is a hard published requirement, restated in both robots.txt and llms.txt.
  evidence: https://drinkprime.com/robots.txt, https://drinkprime.com/llms.txt
  id: buyer_approval
  type: out-of-band
- applies_to: https://drinkprime.com (customer account resources)
  authorization_endpoint: https://orders.drinkprime.com/authentication/oauth/authorize
  bearer_methods_supported:
  - header
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
  description: Shopify Customer Accounts OAuth 2.0 / OpenID Connect, for a shopper acting on their own account. Authorization code flow with PKCE.
  end_session_endpoint: https://orders.drinkprime.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_accounts
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/60993569009
  jwks_uri: https://orders.drinkprime.com/authentication/.well-known/jwks.json
  protected_resource: https://drinkprime.com
  response_types_supported:
  - code
  scopes: See scopes/prime-hydration-scopes.yml
  subject_types_supported:
  - public
  token_endpoint: https://orders.drinkprime.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: prime-hydration-authentication
source_filename: prime-hydration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://drinkprime.com/.well-known/openid-configuration (200),\n  https://drinkprime.com/.well-known/oauth-authorization-server (200),\n  https://drinkprime.com/.well-known/oauth-protected-resource (200), and an anonymous\n  tools/list against https://drinkprime.com/api/ucp/mcp (200) - probed 2026-08-26.\nnote: >-\n  Derived from probed metadata, not from an OpenAPI - Prime Hydration publishes no OpenAPI, so\n  derive-authentication.py had nothing to read. Two distinct auth postures coexist on this\n  provider.\nschemes:\n- id: none\n  type: none\n  applies_to: https://drinkprime.com/api/ucp/mcp\n  description: >-\n    The UCP shopping MCP endpoint answers tools/list anonymously - no Authorization header, no\n    API key, no OAuth challenge. Catalog search/lookup, cart and checkout construction are all\n    reachable without credentials.\n  evidence: >-\n    POST /api/ucp/mcp with no Authorization header returned HTTP 200\
  \ and the full 13-tool\n    manifest with inputSchemas.\n  identity_substitute: >-\n    Instead of a credential, every tool requires meta.ucp-agent.profile - a URI identifying the\n    calling agent. This is agent attestation/discovery, not authentication: it is unverified\n    caller-asserted metadata and grants no privilege.\n- id: buyer_approval\n  type: out-of-band\n  applies_to: complete_checkout\n  description: >-\n    Payment is authorized by the human buyer, not by the agent. complete_checkout additionally\n    requires meta.idempotency-key. Buyer approval is a hard published requirement, restated in\n    both robots.txt and llms.txt.\n  evidence: https://drinkprime.com/robots.txt, https://drinkprime.com/llms.txt\n- id: shopify_customer_accounts\n  type: openIdConnect\n  applies_to: https://drinkprime.com (customer account resources)\n  description: >-\n    Shopify Customer Accounts OAuth 2.0 / OpenID Connect, for a shopper acting on their own\n    account. Authorization code flow\
  \ with PKCE.\n  issuer: https://shopify.com/authentication/60993569009\n  authorization_endpoint: https://orders.drinkprime.com/authentication/oauth/authorize\n  token_endpoint: https://orders.drinkprime.com/authentication/oauth/token\n  end_session_endpoint: https://orders.drinkprime.com/authentication/logout\n  jwks_uri: https://orders.drinkprime.com/authentication/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: See scopes/prime-hydration-scopes.yml\n  bearer_methods_supported: [header]\n  protected_resource: https://drinkprime.com\nregistration:\n  self_service:\
  \ false\n  note: >-\n    There is no developer signup, API key issuance, or client registration surface. The MCP\n    endpoint needs no registration; the Customer Accounts client is a Shopify-issued client for\n    the storefront, not something a third party can provision here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prime-hydration/refs/heads/main/authentication/prime-hydration-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Food and Beverage
- Retail
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Sports Nutrition
---
