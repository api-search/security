---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Oatside Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oatside declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Oatside
provider_slug: oatside
scheme_count: 3
schemes:
- applies_to:
  - tools/list
  - initialize
  - GET /.well-known/ucp
  - GET /products.json
  - GET /collections/{handle}/products.json
  evidence: Anonymous POST tools/list returned HTTP 200 with the full 13-tool manifest on 2026-08-26; no Authorization header was sent.
  id: none
  type: none
- applies_to:
  - tools/call (every tool)
  description: Every tool inputSchema declares a required `meta` object containing `ucp-agent.profile`, a URI the server dereferences to identify the calling agent. This is agent identity, not user authentication or authorization.
  evidence: POST tools/call name=search_catalog with empty arguments returned the -32001 / invalid_profile_url error on 2026-08-26.
  failure_mode:
    data_code: invalid_profile_url
    data_content: 'Unable to fetch agent profile: Missing profile uri'
    jsonrpc_code: -32001
    message: UCP discovery failed
  id: ucp-agent-profile
  in: body
  parameter: meta.ucp-agent.profile
  required: true
  type: agent-identity
- applies_to:
  - complete_checkout
  description: Payment is authorized by the buyer through a payment handler, not by an agent credential. The provider's agents.md and robots.txt both state that agents must not complete checkout, payment or order placement without explicit, contemporaneous human approval, and point unattended shoppers at the Shop Pay skill instead.
  id: buyer-approval
  payment_handlers:
  - com.google.pay
  - dev.shopify.card
  - dev.shopify.shop_pay
  source: https://shop.oatside.com/agents.md
  type: human-in-the-loop
slug: oatside-authentication
source_filename: oatside-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://shop.oatside.com/api/ucp/mcp + https://shop.oatside.com/agents.md\napi: Oatside SG Storefront UCP / MCP\nsummary: >-\n  The storefront's agent surface is anonymous at the protocol level — there is no API key,\n  no OAuth flow and no bearer token. Identity is carried instead by a UCP agent profile\n  URI supplied in every tool call, and the money-moving step is gated on a human, not on a\n  credential.\nschemes:\n- id: none\n  type: none\n  applies_to:\n  - tools/list\n  - initialize\n  - GET /.well-known/ucp\n  - GET /products.json\n  - GET /collections/{handle}/products.json\n  evidence: >-\n    Anonymous POST tools/list returned HTTP 200 with the full 13-tool manifest on\n    2026-08-26; no Authorization header was sent.\n- id: ucp-agent-profile\n  type: agent-identity\n  in: body\n  parameter: meta.ucp-agent.profile\n  required: true\n  applies_to:\n  - tools/call (every tool)\n  description: >-\n    Every tool inputSchema\
  \ declares a required `meta` object containing `ucp-agent.profile`,\n    a URI the server dereferences to identify the calling agent. This is agent identity,\n    not user authentication or authorization.\n  failure_mode:\n    jsonrpc_code: -32001\n    message: UCP discovery failed\n    data_code: invalid_profile_url\n    data_content: 'Unable to fetch agent profile: Missing profile uri'\n  evidence: >-\n    POST tools/call name=search_catalog with empty arguments returned the -32001 /\n    invalid_profile_url error on 2026-08-26.\n- id: buyer-approval\n  type: human-in-the-loop\n  applies_to:\n  - complete_checkout\n  description: >-\n    Payment is authorized by the buyer through a payment handler, not by an agent\n    credential. The provider's agents.md and robots.txt both state that agents must not\n    complete checkout, payment or order placement without explicit, contemporaneous human\n    approval, and point unattended shoppers at the Shop Pay skill instead.\n  payment_handlers:\n\
  \  - com.google.pay\n  - dev.shopify.card\n  - dev.shopify.shop_pay\n  source: https://shop.oatside.com/agents.md\noauth: false\nopenid_connect: false\napi_keys: false\nmutual_tls: false\nnotes:\n- /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource\n  return 404 on both hosts — the MCP endpoint publishes no OAuth metadata because it\n  requires none for the tool surface probed.\n- No scopes/ artifact is emitted: there is no OAuth surface, so there is no scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oatside/refs/heads/main/authentication/oatside-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Oat Milk
- Plant Based
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Retail
- Singapore
- Southeast Asia
---
