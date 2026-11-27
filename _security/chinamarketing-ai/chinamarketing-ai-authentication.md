---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chinamarketing-ai-openapi-generated.yml
  format: yaml
  label: China Marketing AI API
  slug: chinamarketing-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chinamarketing-ai/openapi/_ae-authored/chinamarketing-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: China Marketing AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: China Marketing AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: China Marketing AI
provider_slug: chinamarketing-ai
scheme_count: 1
schemes:
- description: 'Paid routes are authorised by an x402 payment proof sent in the `x402-payment` request header (docs example: -H "x402-payment: <payment_proof>"). "Current paid routes use x402 payment proof. No API key is required unless a future route explicitly states otherwise." An unpaid request returns HTTP 402 with machine-readable payment requirements; the client parses them and retries with proof.'
  header: x402-payment
  in: header
  name: x402-payment
  type: apiKey
  x-protocol: x402
slug: chinamarketing-ai-authentication
source_filename: chinamarketing-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://www.chinamarketing.ai/developers/docs\ndocs: https://www.chinamarketing.ai/developers/docs\nschemes:\n- name: x402-payment\n  type: apiKey\n  in: header\n  header: x402-payment\n  description: >-\n    Paid routes are authorised by an x402 payment proof sent in the `x402-payment` request header (docs example:\n    -H \"x402-payment: <payment_proof>\"). \"Current paid routes use x402 payment proof. No API key is required unless a\n    future route explicitly states otherwise.\" An unpaid request returns HTTP 402 with machine-readable payment\n    requirements; the client parses them and retries with proof.\n  x-protocol: x402\napi_keys: false\noauth2: false\nnote: Modelled as an apiKey-in-header scheme for tooling only; it is a per-request payment proof, not a credential issued to an account.\n"
source_yaml_url: https://artifacts.apis.io/chinamarketing-ai/authentication/chinamarketing-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Marketing
- China
- Generative Engine Optimization
- Market Intelligence
- MCP
- AI Agents
- Brand Visibility
---
