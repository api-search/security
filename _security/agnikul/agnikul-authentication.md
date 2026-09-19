---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Agnikul Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agnikul Cosmos declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Agnikul Cosmos
provider_slug: agnikul
scheme_count: 4
schemes:
- endpoint: https://shop.agnikul.in/api/ucp/mcp
  evidence:
    http_status: 200
    request: POST tools/list with no Authorization header
    result: 13 tools returned with full inputSchemas
  id: none
  note: No API key, bearer token or client credential is required or accepted for tool discovery or for catalog, cart and checkout operations.
  surface: Agnikul Cosmos Store Commerce MCP API
  type: none
  verified: probed
- format: object carrying the agent's UCP profile URI
  id: ucp-agent-profile
  location: request body — meta.ucp-agent
  note: 'Not authentication in the credential sense, but a required identity input on all 13 tools: every inputSchema lists meta as required and meta.required includes "ucp-agent". The server identifies the calling agent, not the user.'
  required: true
  surface: Agnikul Cosmos Store Commerce MCP API
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
    gateway_merchant_id: '85860712758'
    handler: com.google.pay
    id: gpay
    merchant_id: '16708973830884969730'
    merchant_name: Cosmos Store
    merchant_origin: shop.agnikul.in
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
  id: payment-instrument
  location: request body — checkout payment instruments
  note: 'The store''s robots.txt and agents.md both state the rule explicitly: "Checkouts are for humans. Do NOT complete checkout, payment, or order placement automatically ... without an explicit, contemporaneous human approval step."'
  required: true
  shop_pay_absent: true
  shop_pay_note: Unlike most Shopify UCP merchants, this store's profile declares only two payment handlers — dev.shopify.shop_pay is NOT advertised — while the store's own agents.md tells agents to route through Shop Pay when they cannot get contemporaneous buyer approval. The advice and the declared handler set disagree.
  surface: Agnikul Cosmos Store Commerce MCP API — complete_checkout
  type: buyer-authorization
  verified: probed
- authorization_endpoint: https://shopify.com/authentication/85860712758/oauth/authorize
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
  discovery: https://shop.agnikul.in/.well-known/openid-configuration
  end_session_endpoint: https://shopify.com/authentication/85860712758/logout
  id: shopify-customer-account-oauth
  id_token_signing_algs:
  - RS256
  issuer: https://shopify.com/authentication/85860712758
  jwks_uri: https://shopify.com/authentication/85860712758/.well-known/jwks.json
  note: Platform-operated (Shopify customer accounts) and, unlike some merchants, NOT re-hosted on an Agnikul subdomain — every endpoint points straight at shopify.com. Client registration is not publicly documented by Agnikul; there is no self-service developer console on any Agnikul host.
  pkce:
  - S256
  response_types:
  - code
  scopes_file: scopes/agnikul-scopes.yml
  subject_types:
  - public
  subtype: openIdConnect
  surface: Cosmos Store customer accounts (order history, saved addresses)
  token_endpoint: https://shopify.com/authentication/85860712758/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  verified: probed
slug: agnikul-authentication
source_filename: agnikul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://shop.agnikul.in/.well-known/openid-configuration (200),\n  https://shop.agnikul.in/.well-known/oauth-protected-resource (200), anonymous MCP initialize and\n  tools/list against https://shop.agnikul.in/api/ucp/mcp (200), and\n  https://shop.agnikul.in/agents.md (200)\nname: Agnikul authentication profile\nslug: agnikul\n\nsummary: >-\n  Agnikul publishes no API keys and runs no developer key-issuance program on any host. Its one\n  programmable surface — the Cosmos Store commerce MCP endpoint — is anonymous: initialize,\n  tools/list, catalog search, product lookup, cart and checkout creation all succeed with no\n  credential. Authorization moves to the payment step rather than the transport step: completing a\n  checkout requires a buyer-approved payment instrument and an idempotency key. A separate OAuth 2.0\n  / OpenID Connect authorization server exists for store customer accounts. The launch-services\n  business\
  \ at agnikul.in has no authenticated surface at all — no login, no portal, no account system.\n\nschemes:\n- id: none\n  surface: Agnikul Cosmos Store Commerce MCP API\n  endpoint: https://shop.agnikul.in/api/ucp/mcp\n  type: none\n  verified: probed\n  evidence:\n    request: 'POST tools/list with no Authorization header'\n    http_status: 200\n    result: 13 tools returned with full inputSchemas\n  note: >-\n    No API key, bearer token or client credential is required or accepted for tool discovery or for\n    catalog, cart and checkout operations.\n\n- id: ucp-agent-profile\n  surface: Agnikul Cosmos Store Commerce MCP API\n  type: agent-identity\n  required: true\n  location: request body — meta.ucp-agent\n  format: object carrying the agent's UCP profile URI\n  verified: probed\n  note: >-\n    Not authentication in the credential sense, but a required identity input on all 13 tools: every\n    inputSchema lists meta as required and meta.required includes \"ucp-agent\". The server\
  \ identifies\n    the calling agent, not the user.\n\n- id: payment-instrument\n  surface: Agnikul Cosmos Store Commerce MCP API — complete_checkout\n  type: buyer-authorization\n  required: true\n  location: request body — checkout payment instruments\n  verified: probed\n  handlers:\n  - id: gpay\n    handler: com.google.pay\n    version: '2026-01-11'\n    merchant_name: Cosmos Store\n    merchant_id: '16708973830884969730'\n    merchant_origin: shop.agnikul.in\n    gateway: shopify\n    gateway_merchant_id: '85860712758'\n    card_networks: [VISA, MASTERCARD, AMEX, DISCOVER]\n    auth_methods: [PAN_ONLY, CRYPTOGRAM_3DS]\n    billing_address_required: true\n  - id: shopify.card\n    handler: dev.shopify.card\n    version: '2026-01-15'\n    card_brands: [visa, master, american_express, discover, diners_club]\n  shop_pay_absent: true\n  shop_pay_note: >-\n    Unlike most Shopify UCP merchants, this store's profile declares only two payment handlers —\n    dev.shopify.shop_pay is NOT advertised\
  \ — while the store's own agents.md tells agents to route\n    through Shop Pay when they cannot get contemporaneous buyer approval. The advice and the declared\n    handler set disagree.\n  note: >-\n    The store's robots.txt and agents.md both state the rule explicitly: \"Checkouts are for humans.\n    Do NOT complete checkout, payment, or order placement automatically ... without an explicit,\n    contemporaneous human approval step.\"\n\n- id: shopify-customer-account-oauth\n  surface: Cosmos Store customer accounts (order history, saved addresses)\n  type: oauth2\n  subtype: openIdConnect\n  verified: probed\n  issuer: https://shopify.com/authentication/85860712758\n  discovery: https://shop.agnikul.in/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/85860712758/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/85860712758/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/85860712758/logout\n\
  \  jwks_uri: https://shopify.com/authentication/85860712758/.well-known/jwks.json\n  response_types: [code]\n  pkce: ['S256']\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_algs: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes_file: scopes/agnikul-scopes.yml\n  note: >-\n    Platform-operated (Shopify customer accounts) and, unlike some merchants, NOT re-hosted on an\n    Agnikul subdomain — every endpoint points straight at shopify.com. Client registration is not\n    publicly documented by Agnikul; there is no self-service developer console on any Agnikul host.\n\nprotected_resource:\n  source: https://shop.agnikul.in/.well-known/oauth-protected-resource\n  resource: https://shop.agnikul.in\n  authorization_servers:\n  - https://shopify.com/authentication/85860712758\n  bearer_methods_supported: [header]\n  rfc: RFC 9728\n\nlaunch_services_surface:\n  host: agnikul.in\n\
  \  authenticated_surface: none\n  probed:\n  - url: https://agnikul.in/.well-known/openid-configuration\n    http_status: 404\n  - url: https://agnikul.in/.well-known/oauth-authorization-server\n    http_status: 404\n  note: >-\n    No customer portal, no mission dashboard, no login of any kind. Launch enquiries are a public\n    HTML form at https://agnikul.in/book/ that routes to payloadpeople@agnikul.in.\n\ngaps:\n- No security.txt and no published vulnerability-disclosure contact on any Agnikul host.\n- No developer portal, no API key issuance, no documented client registration for the OAuth server.\n- >-\n  The store recommends Shop Pay as the fallback for agents that cannot obtain contemporaneous buyer\n  approval, but does not advertise the dev.shopify.shop_pay handler in its UCP profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agnikul/refs/heads/main/authentication/agnikul-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Aerospace
- Space
- Launch Services
- Satellite
- Manufacturing
- Additive Manufacturing
- India
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
