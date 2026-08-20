---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Boosted Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boosted Commerce declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Boosted Commerce
provider_slug: boosted-commerce
scheme_count: 4
schemes:
- applies_to:
  - tools/list
  - search_catalog
  - lookup_catalog
  - get_product
  - create_cart
  - get_cart
  - update_cart
  - cancel_cart
  - create_checkout
  - get_checkout
  - update_checkout
  - cancel_checkout
  - get_order
  evidence: POST https://primelabs.org/api/ucp/mcp with no Authorization header returned HTTP 200 and a full 13-tool manifest on 2026-08-08.
  id: anonymous
  type: none
- description: Every tool call must carry a `meta.ucp-agent.profile` URI identifying the calling agent for UCP discovery. This identifies the agent; it does not authenticate or authorize it.
  evidence: '`meta.ucp-agent` is a required property of every one of the 13 tool inputSchemas.'
  id: ucp-agent-profile
  in: request body
  parameter: meta.ucp-agent.profile
  required: true
  type: agentIdentity
- applies_to:
  - complete_checkout
  description: Payment completion requires explicit, contemporaneous buyer approval. Agents that cannot obtain it are instructed to route the purchase through Shop Pay via the Shop skill instead.
  evidence: '"Checkout requires human approval. Agents must not complete payment without explicit buyer consent." — https://primelabs.org/agents.md'
  id: buyer-approval
  required: true
  type: humanInTheLoop
- description: Payment instruments are supplied through UCP payment handlers declared in the store's /.well-known/ucp profile, not through credentials issued by Boosted Commerce.
  handlers:
  - id: com.google.pay
    version: '2026-01-11'
  - id: dev.shopify.card
  id: payment-handlers
  type: delegatedPayment
slug: boosted-commerce-authentication
source_filename: boosted-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://primelabs.org/agents.md + live unauthenticated POST to https://primelabs.org/api/ucp/mcp\nnote: >-\n  Boosted Commerce publishes no API keys, OAuth client registration, or developer accounts. The\n  agent-commerce surface on its brand storefronts is deliberately anonymous: `tools/list` and the\n  catalog/cart/checkout tools were exercised with no credentials of any kind. Authorization is not\n  carried by a token at all — it is carried by the buyer, at the moment of payment, through a UCP\n  payment handler. Absence of an auth scheme here is the design, not a gap.\nschemes:\n- id: anonymous\n  type: none\n  applies_to:\n  - tools/list\n  - search_catalog\n  - lookup_catalog\n  - get_product\n  - create_cart\n  - get_cart\n  - update_cart\n  - cancel_cart\n  - create_checkout\n  - get_checkout\n  - update_checkout\n  - cancel_checkout\n  - get_order\n  evidence: >-\n    POST https://primelabs.org/api/ucp/mcp with no Authorization\
  \ header returned HTTP 200 and a full\n    13-tool manifest on 2026-08-08.\n- id: ucp-agent-profile\n  type: agentIdentity\n  in: request body\n  parameter: meta.ucp-agent.profile\n  required: true\n  description: >-\n    Every tool call must carry a `meta.ucp-agent.profile` URI identifying the calling agent for UCP\n    discovery. This identifies the agent; it does not authenticate or authorize it.\n  evidence: '`meta.ucp-agent` is a required property of every one of the 13 tool inputSchemas.'\n- id: buyer-approval\n  type: humanInTheLoop\n  applies_to:\n  - complete_checkout\n  required: true\n  description: >-\n    Payment completion requires explicit, contemporaneous buyer approval. Agents that cannot obtain\n    it are instructed to route the purchase through Shop Pay via the Shop skill instead.\n  evidence: >-\n    \"Checkout requires human approval. Agents must not complete payment without explicit buyer\n    consent.\" — https://primelabs.org/agents.md\n- id: payment-handlers\n\
  \  type: delegatedPayment\n  handlers:\n  - id: com.google.pay\n    version: '2026-01-11'\n  - id: dev.shopify.card\n  description: >-\n    Payment instruments are supplied through UCP payment handlers declared in the store's\n    /.well-known/ucp profile, not through credentials issued by Boosted Commerce.\noauth2: false\nopenid_connect: false\napi_keys: false\nmutual_tls: false\ndocs: https://primelabs.org/agents.md\nx-evidence:\n- url: https://primelabs.org/api/ucp/mcp\n  method: POST\n  http_status: 200\n  fetched: '2026-08-08'\n- url: https://primelabs.org/.well-known/ucp\n  http_status: 200\n  fetched: '2026-08-08'\n- url: https://boostedcommerce.com/.well-known/openid-configuration\n  http_status: 403\n  fetched: '2026-08-08'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boosted-commerce/refs/heads/main/authentication/boosted-commerce-authentication.yml
summary_line: 4 schemes
tags:
- Company
- E-Commerce
- Retail
- Consumer Packaged Goods
- Health and Wellness
- Supplements
- Beauty
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Direct to Consumer
---
