---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Skyfire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skyfire secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Skyfire
provider_slug: skyfire
scheme_count: 2
schemes:
- description: Single header used for every Skyfire REST API request. The value is a role-specific key — Buyer agent, Seller agent, or Enterprise Admin user. Keys are environment-specific (a Sandbox key only works against Sandbox).
  in: header
  name: SkyfireApiKey
  parameter: skyfire-api-key
  roles:
  - role: buyer
    use: Create tokens; inspect the buyer's own tokens, charges, and wallet.
  - role: seller
    use: Manage seller services; charge pay/kya-pay tokens after delivery.
  - role: enterprise-admin
    use: Manage organization users (create/list/activate); not token or service ops.
  type: apiKey
- description: Token-passing header a buyer agent presents to a SELLER SERVICE (not the core Skyfire API). Carries a kya, pay, or kya-pay KYAPay token. Skyfire recommends this dedicated header over Authorization to avoid conflicts with existing auth middleware. Sellers validate it against the issuer JWKS.
  in: header
  name: SkyfirePayId
  parameter: skyfire-pay-id
  type: apiKey
slug: skyfire-authentication
source_filename: skyfire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.skyfire.xyz/reference/api-authentication\ndocs: https://docs.skyfire.xyz/reference/api-authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_name: skyfire-api-key\n  token_format: JWT (JWS ES256, verified against issuer JWKS)\nschemes:\n- name: SkyfireApiKey\n  type: apiKey\n  in: header\n  parameter: skyfire-api-key\n  description: >-\n    Single header used for every Skyfire REST API request. The value is a\n    role-specific key — Buyer agent, Seller agent, or Enterprise Admin user.\n    Keys are environment-specific (a Sandbox key only works against Sandbox).\n  roles:\n  - role: buyer\n    use: Create tokens; inspect the buyer's own tokens, charges, and wallet.\n  - role: seller\n    use: Manage seller services; charge pay/kya-pay tokens after delivery.\n  - role: enterprise-admin\n    use: Manage organization users (create/list/activate); not token or service ops.\n- name: SkyfirePayId\n\
  \  type: apiKey\n  in: header\n  parameter: skyfire-pay-id\n  description: >-\n    Token-passing header a buyer agent presents to a SELLER SERVICE (not the\n    core Skyfire API). Carries a kya, pay, or kya-pay KYAPay token. Skyfire\n    recommends this dedicated header over Authorization to avoid conflicts with\n    existing auth middleware. Sellers validate it against the issuer JWKS.\ntoken_types:\n- id: kya\n  description: Identity-only (Know Your Agent) token.\n- id: pay\n  description: Payment-only token.\n- id: kya-pay\n  description: Combined identity + payment token.\nverification:\n  method: JWT signature verification against issuer JWKS\n  jwks:\n    production: https://app.skyfire.xyz/.well-known/jwks.json\n    sandbox: https://app-sandbox.skyfire.xyz/.well-known/jwks.json\n  issuer:\n    production: https://app.skyfire.xyz\n    sandbox: https://app-sandbox.skyfire.xyz\n  cache_recommendation: 60 minutes\ntroubleshooting:\n- symptom: 401 NOT_AUTHORIZED\n  cause: Key not recognized\
  \ (typo, invalid, or wrong environment).\n- symptom: 400 BAD_REQUEST\n  cause: Valid key but wrong role for the action (e.g. seller key creating a token).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyfire/refs/heads/main/authentication/skyfire-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- Agent Payments
- Identity
- Payments
- Authentication
- Stablecoin
- MCP
- Agentic Commerce
- Know Your Agent
---
