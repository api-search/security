---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CoverBureau Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoverBureau declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CoverBureau
provider_slug: coverbureau-com
scheme_count: 1
schemes:
- description: No account or API key. "An unpaid call returns 402 with a payment challenge; pay it and retry the same request. This is the standard x402 flow, so any x402-capable client handles it for you." The 402 challenge names scheme exact, network eip155:8453 (Base mainnet), the amount and the USDC asset.
  name: x402
  settlement: USDC on Base mainnet
  spec: https://x402.org
  type: payment
slug: coverbureau-com-authentication
source_filename: coverbureau-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coverbureau.com/\ndocs: https://coverbureau.com/\nschemes:\n- name: x402\n  type: payment\n  description: No account or API key. \"An unpaid call returns 402 with a payment challenge; pay it and retry the same request. This is the standard x402 flow, so any x402-capable client handles it for you.\" The 402 challenge names scheme exact, network eip155:8453 (Base mainnet), the amount and the USDC asset.\n  spec: https://x402.org\n  settlement: USDC on Base mainnet\napi_key: false\nsignup_required: false\nresponse_signing:\n  algorithm: Ed25519\n  canonicalization: RFC 8785 (JCS)\n  jwks: https://coverbureau.com/.well-known/jwks.json\n  description: Every response is returned in a signed envelope containing the payload, an Ed25519 signature over the canonical JSON of the payload, the key id and an issued-at timestamp.\n"
source_yaml_url: https://artifacts.apis.io/coverbureau-com/authentication/coverbureau-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Insurance
- Certificates of Insurance
- Compliance
- MCP
- AI Agents
- x402
- Payments
---
