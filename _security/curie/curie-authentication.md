---
api_key_in: []
api_specs:
- filename: curie-openapi.json
  format: json
  label: Curie 3D Product Commerce API
  slug: curie-3d-product-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curie/refs/heads/main/openapi/curie-openapi.json
auth_types:
- none
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Curie Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Curie secures its APIs with none, http-bearer, and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Curie
provider_slug: curie
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code flow. Requires Curie Pro subscription.
  flows:
  - authorizationUrl: https://chat.curie.app/api/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://chat.curie.app/api/oauth/token
  name: oauth2
  sources:
  - openapi/curie-openapi.json
  type: oauth2
slug: curie-authentication
source_filename: curie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/curie-openapi.json\ndocs: https://chat.curie.app/llms.txt\nnotes: >-\n  Tiered access model (per published llms.txt + .well-known/mcp.json). Free\n  public tier requires NO auth for discovery and most MCP tool calls / REST\n  catalog reads (matches Shopify Storefront MCP behaviour), rate-limited to\n  100 req/min per IP. A Pro Bearer token (OAuth 2.0 authorization-code, issued\n  out-of-band) is required only for premium tools such as initiate_checkout and\n  private-merchant-data reads, rate-limited to 1000 req/min per subscriber.\n  Wishlist / aggregate-cart tools resolve identity from an Authorization Bearer\n  JWT or an X-Curie-Device header.\nsummary:\n  types:\n  - none\n  - http-bearer\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://chat.curie.app/api/oauth/authorize\n    tokenUrl:\
  \ https://chat.curie.app/api/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authorization code flow. Requires Curie Pro subscription.\n  sources:\n  - openapi/curie-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curie/refs/heads/main/authentication/curie-authentication.yml
summary_line: none/http-bearer/oauth2 · 1 scheme
tags:
- Company
- Commerce
- E-Commerce
- Shopify
- Artificial Intelligence
- Model Context Protocol
- Agentic Commerce
- Product Discovery
- 3D
---
