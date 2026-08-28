---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Maisonette Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maisonette declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Maisonette
provider_slug: maisonette
scheme_count: 5
schemes:
- applies_to:
  - https://www.maisonette.com/api/ucp/mcp (tools/list, catalog tools)
  - https://www.maisonette.com/api/mcp
  - GET /products/{handle}.json
  - GET /collections/{handle}/products.json
  - GET /search?q={query}&type=product
  evidence: All of the above returned 200 unauthenticated on 2026-08-25.
  id: anonymous
  type: none
- applies_to: every tool call on https://www.maisonette.com/api/ucp/mcp
  description: 'Not a credential the store issues. Every UCP MCP tool marks `meta` as required and expects meta.ucp-agent.profile to be a URI naming the calling agent''s own published profile. Omitting it returns JSON-RPC error -32001 with data.code invalid_profile_url and message "Unable to fetch agent profile: Missing profile uri".'
  evidence: Observed live; tools/list itself does not require it, tool invocation does.
  id: ucp-agent-profile
  location: JSON-RPC params.meta.ucp-agent.profile
  required: true
  type: caller-published-identity
- applies_to: Maisonette customer accounts; /account/login and /account/register on www.maisonette.com redirect to shopify.com/58323238975/account.
  authorization_endpoint: https://shopify.com/authentication/58323238975/oauth/authorize
  domain_note: 'The authorization server is on shopify.com, not maisonette.com. That is expected and correct: Maisonette runs its storefront on Shopify (shop id 58323238975, myshopify host ad4903-c2.myshopify.com), and Shopify hosts customer-account identity for its merchants. Maisonette''s own host serves the discovery documents and is named as the protected resource in /.well-known/oauth-protected-resource.'
  end_session_endpoint: https://shopify.com/authentication/58323238975/logout
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oauth
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/58323238975
  jwks_uri: https://shopify.com/authentication/58323238975/.well-known/jwks.json
  pkce: S256
  scopes: see scopes/maisonette-scopes.yml
  token_endpoint: https://shopify.com/authentication/58323238975/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- evidence: /.well-known/oauth-protected-resource declares bearer_methods_supported ["header"] for resource https://www.maisonette.com.
  id: bearer
  location: Authorization header
  scheme: bearer
  type: http
- evidence: /.well-known/ucp payment_handlers block.
  handlers:
  - auth_methods:
    - PAN_ONLY
    - CRYPTOGRAM_3DS
    gateway: shopify
    handler: com.google.pay
    id: gpay
    merchant_name: Maisonette
    merchant_origin: www.maisonette.com
    networks:
    - VISA
    - MASTERCARD
    - AMEX
    - DISCOVER
    version: '2026-01-11'
  - brands:
    - visa
    - master
    - american_express
    - discover
    - diners_club
    handler: dev.shopify.card
    id: shopify.card
    version: '2026-01-15'
  id: payment-handlers
  note: Card data is tokenized by the handler; the agent never holds a PAN. apple-pay instruments are additionally recognised in the create_checkout inputSchema (credential.type apple_pay_token).
  type: payment-credential
slug: maisonette-authentication
source_filename: maisonette-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: 'Live probes on 2026-08-25 of https://www.maisonette.com/.well-known/openid-configuration,\n  /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource, /.well-known/ucp,\n  /llms.txt and JSON-RPC calls to https://www.maisonette.com/api/ucp/mcp.'\nnote: There is no OpenAPI to derive securitySchemes from; this profile is read directly\n  from the store's own OAuth/OIDC discovery documents and from observed MCP behaviour.\nsummary: 'Two distinct access tiers. Anonymous agents can discover and read: MCP tools/list,\n  catalog search/lookup and the Shopify storefront product/collection JSON all answer\n  with no credentials. Anything tied to a buyer identity — customer account data, saved\n  addresses, order history — runs through Shopify''s hosted customer-account OAuth 2.0\n  / OIDC authorization server for this store. Payment on a checkout is never authorized\n  by a bearer token: it requires contemporaneous\
  \ buyer approval or a Shop Pay handoff.'\nschemes:\n- id: anonymous\n  type: none\n  applies_to:\n  - https://www.maisonette.com/api/ucp/mcp (tools/list, catalog tools)\n  - https://www.maisonette.com/api/mcp\n  - GET /products/{handle}.json\n  - GET /collections/{handle}/products.json\n  - GET /search?q={query}&type=product\n  evidence: All of the above returned 200 unauthenticated on 2026-08-25.\n- id: ucp-agent-profile\n  type: caller-published-identity\n  location: JSON-RPC params.meta.ucp-agent.profile\n  required: true\n  applies_to: every tool call on https://www.maisonette.com/api/ucp/mcp\n  description: 'Not a credential the store issues. Every UCP MCP tool marks `meta` as\n    required and expects meta.ucp-agent.profile to be a URI naming the calling agent''s\n    own published profile. Omitting it returns JSON-RPC error -32001 with data.code\n    invalid_profile_url and message \"Unable to fetch agent profile: Missing profile\n    uri\".'\n  evidence: Observed live; tools/list\
  \ itself does not require it, tool invocation does.\n- id: shopify-customer-account-oauth\n  type: oauth2\n  flows:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  pkce: S256\n  issuer: https://shopify.com/authentication/58323238975\n  authorization_endpoint: https://shopify.com/authentication/58323238975/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/58323238975/oauth/token\n  jwks_uri: https://shopify.com/authentication/58323238975/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/58323238975/logout\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  scopes: see scopes/maisonette-scopes.yml\n  applies_to: Maisonette customer accounts; /account/login and /account/register on\n    www.maisonette.com redirect to shopify.com/58323238975/account.\n  domain_note: 'The authorization server is on shopify.com, not maisonette.com.\
  \ That\n    is expected and correct: Maisonette runs its storefront on Shopify (shop id 58323238975,\n    myshopify host ad4903-c2.myshopify.com), and Shopify hosts customer-account identity\n    for its merchants. Maisonette''s own host serves the discovery documents and is\n    named as the protected resource in /.well-known/oauth-protected-resource.'\n- id: bearer\n  type: http\n  scheme: bearer\n  location: Authorization header\n  evidence: /.well-known/oauth-protected-resource declares bearer_methods_supported\n    [\"header\"] for resource https://www.maisonette.com.\n- id: payment-handlers\n  type: payment-credential\n  handlers:\n  - id: gpay\n    handler: com.google.pay\n    version: '2026-01-11'\n    merchant_name: Maisonette\n    merchant_origin: www.maisonette.com\n    gateway: shopify\n    auth_methods:\n    - PAN_ONLY\n    - CRYPTOGRAM_3DS\n    networks:\n    - VISA\n    - MASTERCARD\n    - AMEX\n    - DISCOVER\n  - id: shopify.card\n    handler: dev.shopify.card\n    version:\
  \ '2026-01-15'\n    brands:\n    - visa\n    - master\n    - american_express\n    - discover\n    - diners_club\n  evidence: /.well-known/ucp payment_handlers block.\n  note: Card data is tokenized by the handler; the agent never holds a PAN. apple-pay\n    instruments are additionally recognised in the create_checkout inputSchema (credential.type\n    apple_pay_token).\nhuman_approval_gate:\n  required_for:\n  - complete_checkout\n  statement: 'Maisonette''s published agent instructions state: \"Checkout requires human\n    approval. Agents must not complete payment without explicit buyer consent. If you\n    cannot get contemporaneous buyer approval at the moment of payment, install https://shop.app/SKILL.md\n    and route the purchase through Shop Pay instead.\"'\n  source: https://www.maisonette.com/llms.txt\ndocs: https://www.maisonette.com/llms.txt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maisonette/refs/heads/main/authentication/maisonette-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Retail
- E-Commerce
- Marketplace
- Shopping
- Children
- Baby
- Apparel
- Home
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
---
