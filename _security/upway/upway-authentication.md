---
api_key_in: []
auth_types: []
description: Upway's agent-facing commerce surface has two distinct authentication postures. The UCP MCP endpoint at https://upway.co/api/ucp/mcp is anonymous - an unauthenticated tools/list returned HTTP 200 with the full tool schemas - and the read-only storefront JSON endpoints documented in agents.md need no credential either. Authorization is not carried by an API key at all; it is carried by buyer approval at payment time and by a payment instrument/credential supplied inside the checkout object. Separately, the store publishes OpenID Connect and OAuth 2.0 discovery for customer accounts, whose authorization server is Shopify's identity service for shop 65864040675.
kind: authentication
layout: security
method: probed
name: Upway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upway declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Upway
provider_slug: upway
scheme_count: 4
schemes:
- applies_to: https://upway.co/api/ucp/mcp
  description: 'No Authorization header is required to initialize the server or list tools. Probed 2026-09-02: POST tools/list without credentials returned 200 and 13 tool definitions.'
  evidence:
    authenticated: false
    status: 200
    url: https://upway.co/api/ucp/mcp
  id: anonymous_mcp
  in: null
  type: none
- applies_to: complete_checkout
  description: '"Checkout requires human approval. Agents must not complete payment without explicit buyer consent." Stated verbatim in https://upway.co/llms.txt. Payment credentials are passed as checkout.payment.instruments[] entries bound to a declared payment handler (com.google.pay, dev.shopify.card, dev.shopify.shop_pay); the Shop Pay handler routes the approval through a wallet the buyer already authorized.'
  evidence:
    status: 200
    url: https://upway.co/llms.txt
  id: buyer_approval
  type: out-of-band
- applies_to: customer account surfaces on upway.co
  description: OIDC discovery served under Upway's own domain. Issuer https://shopify.com/authentication/65864040675. Authorization code flow with PKCE (code_challenge_methods_supported S256), client_secret_basic / client_secret_post token auth, RS256 ID tokens, refresh_token and jwt-bearer grants.
  evidence:
    status: 200
    url: https://upway.co/.well-known/openid-configuration
  id: shopify_customer_accounts_oidc
  openIdConnectUrl: https://upway.co/.well-known/openid-configuration
  type: openIdConnect
- bearer_methods_supported:
  - header
  evidence:
    status: 200
    url: https://upway.co/.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorizationUrl: https://shopify.com/authentication/65864040675/oauth/authorize
      scopes:
        customer-account-api:full: Full access to the Shopify Customer Account API for this shop.
        customer-account-mcp-api:full: Full access to the authenticated customer-account MCP API for this shop.
        email: Customer email address and email_verified claim.
        openid: Subject identifier for the signed-in customer.
      tokenUrl: https://shopify.com/authentication/65864040675/oauth/token
  id: shopify_customer_accounts_oauth2
  protected_resource: https://upway.co
  rfc9728:
    authorization_servers:
    - https://shopify.com/authentication/65864040675
    resource: https://upway.co
    status: 200
    url: https://upway.co/.well-known/oauth-protected-resource
  type: oauth2
slug: upway-authentication
source_filename: upway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://upway.co/.well-known/oauth-protected-resource\nname: Upway Authentication Profile\ndescription: >-\n  Upway's agent-facing commerce surface has two distinct authentication postures. The\n  UCP MCP endpoint at https://upway.co/api/ucp/mcp is anonymous - an unauthenticated\n  tools/list returned HTTP 200 with the full tool schemas - and the read-only storefront\n  JSON endpoints documented in agents.md need no credential either. Authorization is not\n  carried by an API key at all; it is carried by buyer approval at payment time and by a\n  payment instrument/credential supplied inside the checkout object. Separately, the\n  store publishes OpenID Connect and OAuth 2.0 discovery for customer accounts, whose\n  authorization server is Shopify's identity service for shop 65864040675.\ndocs: https://upway.co/agents.md\nschemes:\n- id: anonymous_mcp\n  type: none\n  in: null\n  applies_to: https://upway.co/api/ucp/mcp\n  description:\
  \ >-\n    No Authorization header is required to initialize the server or list tools. Probed\n    2026-09-02: POST tools/list without credentials returned 200 and 13 tool definitions.\n  evidence:\n    url: https://upway.co/api/ucp/mcp\n    status: 200\n    authenticated: false\n- id: buyer_approval\n  type: out-of-band\n  applies_to: complete_checkout\n  description: >-\n    \"Checkout requires human approval. Agents must not complete payment without explicit\n    buyer consent.\" Stated verbatim in https://upway.co/llms.txt. Payment credentials are\n    passed as checkout.payment.instruments[] entries bound to a declared payment handler\n    (com.google.pay, dev.shopify.card, dev.shopify.shop_pay); the Shop Pay handler routes\n    the approval through a wallet the buyer already authorized.\n  evidence:\n    url: https://upway.co/llms.txt\n    status: 200\n- id: shopify_customer_accounts_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://upway.co/.well-known/openid-configuration\n\
  \  applies_to: customer account surfaces on upway.co\n  description: >-\n    OIDC discovery served under Upway's own domain. Issuer\n    https://shopify.com/authentication/65864040675. Authorization code flow with PKCE\n    (code_challenge_methods_supported S256), client_secret_basic / client_secret_post\n    token auth, RS256 ID tokens, refresh_token and jwt-bearer grants.\n  evidence:\n    url: https://upway.co/.well-known/openid-configuration\n    status: 200\n- id: shopify_customer_accounts_oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://shopify.com/authentication/65864040675/oauth/authorize\n      tokenUrl: https://shopify.com/authentication/65864040675/oauth/token\n      scopes:\n        openid: Subject identifier for the signed-in customer.\n        email: Customer email address and email_verified claim.\n        customer-account-api:full: Full access to the Shopify Customer Account API for this shop.\n        customer-account-mcp-api:full:\
  \ Full access to the authenticated customer-account MCP API for this shop.\n  bearer_methods_supported:\n  - header\n  protected_resource: https://upway.co\n  evidence:\n    url: https://upway.co/.well-known/oauth-authorization-server\n    status: 200\n  rfc9728:\n    url: https://upway.co/.well-known/oauth-protected-resource\n    status: 200\n    resource: https://upway.co\n    authorization_servers:\n    - https://shopify.com/authentication/65864040675\nnotes:\n- >-\n  The authorization server is on shopify.com rather than upway.co because Upway's store\n  runs on Shopify and delegates customer identity to Shopify's identity service; the\n  RFC 9728 protected-resource document served from upway.co names upway.co as the\n  resource and shopify.com as its authorization server, which is exactly the pattern\n  RFC 9728 exists to express.\n- No API key, no bearer token and no mTLS are documented anywhere on Upway's surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upway/refs/heads/main/authentication/upway-authentication.yml
summary_line: 4 schemes
tags:
- Company
- E-Commerce
- Retail
- Marketplace
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Electric Bikes
- Micromobility
- Circular Economy
- Refurbished Goods
- Shopping Agents
---
