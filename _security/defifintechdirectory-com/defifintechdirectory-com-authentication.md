---
anonymous_access: false
api_key_in: []
api_specs:
- filename: defifintechdirectory-com-coming-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Coming API
  slug: defifintechdirectory-com-coming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-coming-api-openapi.yml
- filename: defifintechdirectory-com-local-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Local API
  slug: defifintechdirectory-com-local-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-local-api-openapi.yml
- filename: defifintechdirectory-com-local-capability-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Local Capability API
  slug: defifintechdirectory-com-local-capability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-local-capability-api-openapi.yml
- filename: defifintechdirectory-com-meta-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Meta API
  slug: defifintechdirectory-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-meta-api-openapi.yml
- filename: defifintechdirectory-com-skill-pack-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Skill Pack API
  slug: defifintechdirectory-com-skill-pack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-skill-pack-api-openapi.yml
- filename: defifintechdirectory-com-tools-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Tools API
  slug: defifintechdirectory-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-tools-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Defifintechdirectory Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeFi Fintech Directory declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DeFi Fintech Directory
provider_slug: defifintechdirectory-com
scheme_count: 2
schemes:
- asset: USDC
  challenge_header: PAYMENT-REQUIRED
  challenge_status: 402
  evidence: No account, no Stripe, no API key for buyers.
  header: PAYMENT-SIGNATURE
  in: header
  mcp_equivalent: _meta["x402/payment"]
  name: x402-payment
  network: eip155:8453
  scheme: exact
  type: payment
- evidence: It requires a session cookie, same-origin requests and a CSRF token for mutations.
  name: human-workspace-session
  note: Production authentication is stated as not connected ("Production authentication, distributed credit storage, private artifact storage and Stripe test checkout are not connected.").
  scope: local-only /api/human browser interface
  type: cookie
slug: defifintechdirectory-com-authentication
source_filename: defifintechdirectory-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://defifintechdirectory.com/how-to-pay.html\n- https://api.defifintechdirectory.com/llms.txt\n- https://api.defifintechdirectory.com/developers\ndocs: https://defifintechdirectory.com/how-to-pay.html\nsummary: >-\n  No API keys or buyer accounts. Paid tool calls are authorized per request with the x402 payment protocol\n  (v2): an unpaid request returns HTTP 402 with a PAYMENT-REQUIRED header, and the client retries with a\n  signed USDC authorization (EIP-3009) in the PAYMENT-SIGNATURE header. The OpenAPI contracts declare no\n  securitySchemes. The browser workspace's /api/human interface uses a session cookie plus CSRF token\n  (not an integration surface; not exercised).\nschemes:\n- name: x402-payment\n  type: payment\n  in: header\n  header: PAYMENT-SIGNATURE\n  challenge_header: PAYMENT-REQUIRED\n  challenge_status: 402\n  network: eip155:8453\n  asset: USDC\n  scheme: exact\n  evidence: \"No account, no Stripe,\
  \ no API key for buyers.\"\n  mcp_equivalent: _meta[\"x402/payment\"]\n- name: human-workspace-session\n  type: cookie\n  scope: local-only /api/human browser interface\n  evidence: \"It requires a session cookie, same-origin requests and a CSRF token for mutations.\"\n  note: Production authentication is stated as not connected (\"Production authentication, distributed credit storage, private artifact storage and Stripe test checkout are not connected.\").\n"
source_yaml_url: https://artifacts.apis.io/defifintechdirectory-com/authentication/defifintechdirectory-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- DeFi
- Fintech
- x402
- Micropayments
- USDC
- Base
- AI Agents
- Directory
- MCP
---
