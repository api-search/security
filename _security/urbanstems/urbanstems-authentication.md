---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Urbanstems Authentication
name_suffix: Authentication
oauth_flows: []
overview: UrbanStems declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: UrbanStems
provider_slug: urbanstems
scheme_count: 4
schemes:
- endpoint: https://274513-24.myshopify.com/api/ucp/mcp
  evidence:
    http_status: 200
    request: POST tools/list with no Authorization header
    result: 13 tools returned with full inputSchemas
  id: none
  note: No API key, bearer token or client credential is required or accepted for tool discovery or for catalog, cart and checkout operations.
  surface: UrbanStems Commerce MCP API
  type: none
  verified: probed
- format: URI
  id: ucp-agent-profile
  location: request body — meta.ucp-agent.profile
  note: 'Not authentication in the credential sense, but it is a required identity input on all 13 tools: every inputSchema lists meta as required, and meta requires ucp-agent, which requires profile — "Agent profile URI for UCP discovery." The server identifies the calling agent, not the user.'
  required: true
  surface: UrbanStems Commerce MCP API
  type: agent-identity
  verified: probed
- handlers:
  - auth_methods:
    - PAN_ONLY
    - CRYPTOGRAM_3DS
    billing_address_required: true
    card_networks:
    - VISA
    - MASTERCARD
    - AMEX
    - DISCOVER
    gateway: shopify
    handler: com.google.pay
    id: gpay
    merchant_id: '16708973830884969730'
    merchant_origin: urbanstems.com
    version: '2026-01-11'
  - card_brands:
    - visa
    - master
    - american_express
    - discover
    - diners_club
    handler: dev.shopify.card
    id: shopify.card
    version: '2026-01-15'
  - handler: dev.shopify.shop_pay
    id: shop_pay
    shop_id: '69340168440'
    version: '2026-04-08'
  id: payment-instrument
  location: request body — checkout.payment.instruments[]
  note: 'complete_checkout requires checkout.payment. Apple Pay instruments are additionally constrained by the schema to type "card" with an apple_pay_token credential and a billing_address. The provider''s own agent instructions state: "Checkout requires human approval. Agents must not complete payment without explicit buyer consent."'
  required: true
  surface: UrbanStems Commerce MCP API — complete_checkout
  type: buyer-authorization
  verified: probed
- authorization_endpoint: https://tracking.urbanstems.com/authentication/oauth/authorize
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
  discovery: https://urbanstems.com/.well-known/openid-configuration
  end_session_endpoint: https://tracking.urbanstems.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oauth
  id_token_signing_algs:
  - RS256
  issuer: https://shopify.com/authentication/69340168440
  jwks_uri: https://tracking.urbanstems.com/authentication/.well-known/jwks.json
  note: Platform-operated (Shopify customer accounts) but published under UrbanStems' own hostnames. Client registration is not publicly documented by UrbanStems; there is no self-service developer console on urbanstems.com.
  pkce:
  - S256
  response_types:
  - code
  scopes_file: scopes/urbanstems-scopes.yml
  subject_types:
  - public
  subtype: openIdConnect
  surface: Customer accounts (order history, saved addresses)
  token_endpoint: https://tracking.urbanstems.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  verified: probed
slug: urbanstems-authentication
source_filename: urbanstems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://urbanstems.com/.well-known/openid-configuration (200),\n  https://urbanstems.com/.well-known/oauth-protected-resource (200), anonymous MCP tools/list and\n  initialize against https://274513-24.myshopify.com/api/ucp/mcp (200), and\n  https://urbanstems.com/agents.md (200)\nname: UrbanStems authentication profile\nslug: urbanstems\n\nsummary: >-\n  UrbanStems publishes no API keys and runs no developer key-issuance program. Its agent-facing\n  commerce API is anonymous: tools/list, catalog search, product lookup, cart and checkout creation\n  all succeed with no credential. Authorization moves to the payment step instead of the transport\n  step — completing a checkout requires a buyer-approved payment instrument and an idempotency key.\n  A separate OAuth 2.0 / OpenID Connect authorization server exists for customer accounts.\n\nschemes:\n- id: none\n  surface: UrbanStems Commerce MCP API\n  endpoint: https://274513-24.myshopify.com/api/ucp/mcp\n\
  \  type: none\n  verified: probed\n  evidence:\n    request: 'POST tools/list with no Authorization header'\n    http_status: 200\n    result: 13 tools returned with full inputSchemas\n  note: >-\n    No API key, bearer token or client credential is required or accepted for tool discovery or for\n    catalog, cart and checkout operations.\n\n- id: ucp-agent-profile\n  surface: UrbanStems Commerce MCP API\n  type: agent-identity\n  required: true\n  location: request body — meta.ucp-agent.profile\n  format: URI\n  verified: probed\n  note: >-\n    Not authentication in the credential sense, but it is a required identity input on all 13 tools:\n    every inputSchema lists meta as required, and meta requires ucp-agent, which requires profile —\n    \"Agent profile URI for UCP discovery.\" The server identifies the calling agent, not the user.\n\n- id: payment-instrument\n  surface: UrbanStems Commerce MCP API — complete_checkout\n  type: buyer-authorization\n  required: true\n  location:\
  \ request body — checkout.payment.instruments[]\n  verified: probed\n  handlers:\n  - id: gpay\n    handler: com.google.pay\n    version: '2026-01-11'\n    merchant_id: '16708973830884969730'\n    merchant_origin: urbanstems.com\n    gateway: shopify\n    card_networks: [VISA, MASTERCARD, AMEX, DISCOVER]\n    auth_methods: [PAN_ONLY, CRYPTOGRAM_3DS]\n    billing_address_required: true\n  - id: shopify.card\n    handler: dev.shopify.card\n    version: '2026-01-15'\n    card_brands: [visa, master, american_express, discover, diners_club]\n  - id: shop_pay\n    handler: dev.shopify.shop_pay\n    version: '2026-04-08'\n    shop_id: '69340168440'\n  note: >-\n    complete_checkout requires checkout.payment. Apple Pay instruments are additionally constrained\n    by the schema to type \"card\" with an apple_pay_token credential and a billing_address. The\n    provider's own agent instructions state: \"Checkout requires human approval. Agents must not\n    complete payment without explicit buyer\
  \ consent.\"\n\n- id: shopify-customer-account-oauth\n  surface: Customer accounts (order history, saved addresses)\n  type: oauth2\n  subtype: openIdConnect\n  verified: probed\n  issuer: https://shopify.com/authentication/69340168440\n  discovery: https://urbanstems.com/.well-known/openid-configuration\n  authorization_endpoint: https://tracking.urbanstems.com/authentication/oauth/authorize\n  token_endpoint: https://tracking.urbanstems.com/authentication/oauth/token\n  end_session_endpoint: https://tracking.urbanstems.com/authentication/logout\n  jwks_uri: https://tracking.urbanstems.com/authentication/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  pkce: ['S256']\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_algs: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes_file:\
  \ scopes/urbanstems-scopes.yml\n  note: >-\n    Platform-operated (Shopify customer accounts) but published under UrbanStems' own hostnames.\n    Client registration is not publicly documented by UrbanStems; there is no self-service developer\n    console on urbanstems.com.\n\nprotected_resource:\n  source: https://urbanstems.com/.well-known/oauth-protected-resource\n  resource: https://urbanstems.com\n  authorization_servers:\n  - https://tracking.urbanstems.com\n  - https://shopify.com/authentication/69340168440\n  bearer_methods_supported: [header]\n  rfc: RFC 9728\n\ngaps:\n- No security.txt and no published vulnerability-disclosure contact on any UrbanStems host.\n- No developer portal, no API key issuance, no documented client registration for the OAuth server.\n- >-\n  The MCP endpoint UrbanStems documents in /llms.txt and /agents.md\n  (https://urbanstems.com/api/ucp/mcp) returns 404; the working endpoint is only discoverable via\n  /.well-known/ucp.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanstems/refs/heads/main/authentication/urbanstems-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Flowers
- Gifting
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Direct to Consumer
---
