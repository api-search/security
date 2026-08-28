---
api_key_in: []
auth_types: []
description: 'Rock The Bells'' agent-facing surfaces are unusually open: both the MCP tool manifest and the full Storefront GraphQL schema were enumerated with no credential of any kind. What is gated is not discovery but MONEY — payment completion is guarded by a human-approval invariant rather than by a token.'
kind: authentication
layout: security
method: probed
name: Rock The Bells Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rock The Bells declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Rock The Bells
provider_slug: rock-the-bells
scheme_count: 5
schemes:
- applies_to:
  - POST https://shop.rockthebells.com/api/ucp/mcp (tools/list)
  - POST https://shop.rockthebells.com/api/2024-10/graphql.json (introspection + public reads)
  - GET https://shop.rockthebells.com/.well-known/ucp
  - GET https://shop.rockthebells.com/products.json
  - GET https://shop.rockthebells.com/collections.json
  evidence: All of the above returned HTTP 200 to an unauthenticated request on 2026-08-26. Full GraphQL introspection (414 types) and the complete 13-tool MCP manifest were both retrieved anonymously.
  id: anonymous-discovery
  type: none
- applies_to: every MCP tool
  description: 'Every one of the 13 MCP tools declares `meta` as a required property, and within it `ucp-agent.profile` — a URI identifying the calling agent — is itself required. This is agent IDENTIFICATION, not authentication: nothing was verified against the profile URI during probing.'
  evidence: mcp/rock-the-bells-mcp-tools.json (inputSchema.properties.meta.required = ["ucp-agent"])
  id: ucp-agent-profile
  location: request body
  parameter: meta.ucp-agent.profile
  required: true
  type: agentIdentity
- description: The Shopify Storefront API convention for authenticated storefront access. NOT required for the public read and introspection surface observed here; it scopes elevated or app-specific access. Recorded as the documented platform scheme, not as something Rock The Bells publishes itself.
  evidence: Shopify Storefront API platform convention; not exercised during this probe.
  id: storefront-access-token
  in: header
  name: X-Shopify-Storefront-Access-Token
  required: false
  type: apiKey
- description: Buyer-account authentication inside the Storefront schema. The Mutation type exposes customerAccessTokenCreate, customerAccessTokenCreateWithMultipass, customerAccessTokenRenew and customerAccessTokenDelete; customer-scoped queries take the resulting token. This authenticates the SHOPPER, not the API consumer.
  evidence: graphql/rock-the-bells-storefront.graphql (Mutation.customerAccessTokenCreate)
  id: customer-access-token
  location: GraphQL mutation argument
  type: bearer
- applies_to:
  - complete_checkout (MCP)
  - cartSubmitForCompletion (GraphQL)
  - shopPayPaymentRequestSessionSubmit (GraphQL)
  description: The store's controlling authorization rule for agents. Payment may not be finalized without an explicit, contemporaneous human approval step — this is stated in BOTH /llms.txt and /robots.txt, and is the invariant that substitutes for an API credential on the write path.
  evidence: 'llms.txt "Important Rules": "Checkout requires human approval. Agents must not complete payment without explicit buyer consent." robots.txt: "Checkouts are for humans. Do NOT complete checkout, payment, or order placement automatically."'
  id: buyer-approval
  required: true
  type: humanInTheLoop
slug: rock-the-bells-authentication
source_filename: rock-the-bells-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://shop.rockthebells.com/api/ucp/mcp,\n  https://shop.rockthebells.com/api/2024-10/graphql.json,\n  https://shop.rockthebells.com/llms.txt\ndescription: >-\n  Rock The Bells' agent-facing surfaces are unusually open: both the MCP tool manifest and the full\n  Storefront GraphQL schema were enumerated with no credential of any kind. What is gated is not\n  discovery but MONEY — payment completion is guarded by a human-approval invariant rather than by\n  a token.\nschemes:\n- id: anonymous-discovery\n  type: none\n  applies_to:\n  - POST https://shop.rockthebells.com/api/ucp/mcp (tools/list)\n  - POST https://shop.rockthebells.com/api/2024-10/graphql.json (introspection + public reads)\n  - GET https://shop.rockthebells.com/.well-known/ucp\n  - GET https://shop.rockthebells.com/products.json\n  - GET https://shop.rockthebells.com/collections.json\n  evidence: >-\n    All of the above returned HTTP 200 to an unauthenticated\
  \ request on 2026-08-26. Full GraphQL\n    introspection (414 types) and the complete 13-tool MCP manifest were both retrieved anonymously.\n- id: ucp-agent-profile\n  type: agentIdentity\n  location: request body\n  parameter: meta.ucp-agent.profile\n  required: true\n  applies_to: every MCP tool\n  description: >-\n    Every one of the 13 MCP tools declares `meta` as a required property, and within it\n    `ucp-agent.profile` — a URI identifying the calling agent — is itself required. This is agent\n    IDENTIFICATION, not authentication: nothing was verified against the profile URI during probing.\n  evidence: mcp/rock-the-bells-mcp-tools.json (inputSchema.properties.meta.required = [\"ucp-agent\"])\n- id: storefront-access-token\n  type: apiKey\n  in: header\n  name: X-Shopify-Storefront-Access-Token\n  required: false\n  description: >-\n    The Shopify Storefront API convention for authenticated storefront access. NOT required for the\n    public read and introspection surface observed\
  \ here; it scopes elevated or app-specific access.\n    Recorded as the documented platform scheme, not as something Rock The Bells publishes itself.\n  evidence: Shopify Storefront API platform convention; not exercised during this probe.\n- id: customer-access-token\n  type: bearer\n  location: GraphQL mutation argument\n  description: >-\n    Buyer-account authentication inside the Storefront schema. The Mutation type exposes\n    customerAccessTokenCreate, customerAccessTokenCreateWithMultipass, customerAccessTokenRenew and\n    customerAccessTokenDelete; customer-scoped queries take the resulting token. This authenticates\n    the SHOPPER, not the API consumer.\n  evidence: graphql/rock-the-bells-storefront.graphql (Mutation.customerAccessTokenCreate)\n- id: buyer-approval\n  type: humanInTheLoop\n  required: true\n  applies_to:\n  - complete_checkout (MCP)\n  - cartSubmitForCompletion (GraphQL)\n  - shopPayPaymentRequestSessionSubmit (GraphQL)\n  description: >-\n    The store's\
  \ controlling authorization rule for agents. Payment may not be finalized without an\n    explicit, contemporaneous human approval step — this is stated in BOTH /llms.txt and\n    /robots.txt, and is the invariant that substitutes for an API credential on the write path.\n  evidence: >-\n    llms.txt \"Important Rules\": \"Checkout requires human approval. Agents must not complete payment\n    without explicit buyer consent.\" robots.txt: \"Checkouts are for humans. Do NOT complete\n    checkout, payment, or order placement automatically.\"\noauth: false\noauth_note: >-\n  No OAuth. Both /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource\n  returned 404 on every host, and the MCP endpoint returned tools rather than an OAuth challenge.\n  scopes/ is therefore intentionally absent for this provider.\ndocs: https://shop.rockthebells.com/llms.txt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rock-the-bells/refs/heads/main/authentication/rock-the-bells-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Retail
- Ecommerce
- Merchandise
- Apparel
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- GraphQL
- Media
- Music
- Hip-Hop
---
