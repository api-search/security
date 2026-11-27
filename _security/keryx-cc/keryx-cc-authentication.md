---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keryx-cc-openapi-generated.yml
  format: yaml
  label: Keryx API
  slug: keryx-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keryx-cc/openapi/_ae-authored/keryx-cc-openapi-generated.yml
auth_types: []
description: 'Authentication: Two modes — x402-only: attach a valid payment-signature header (x402 v2 format). No key needed. Key + x402: mint an API key at /api/keys (SIWE wallet required), then attach both Authorization: Bearer kx_live_… and payment-signature. Key adds identity, rate-limit, and usage metering — it does NOT waive the payment requirement. No free compute.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Keryx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keryx declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Keryx
provider_slug: keryx-cc
scheme_count: 2
schemes:
- evidence: 'x402-only: attach a valid payment-signature header (x402 v2 format). No key needed.'
  header: payment-signature
  location: header
  name: payment-signature
  type: apiKey
- evidence: 'Key + x402: mint an API key at /api/keys (SIWE wallet required), then attach both Authorization: Bearer kx_live_… and payment-signature.'
  header: Authorization
  how_to_obtain: Mint an API key at /api/keys (SIWE wallet required).
  location: header
  name: Authorization
  type: http-bearer
slug: keryx-cc-authentication
source_filename: keryx-cc-authentication.yml
source_heading: Authentication Profile
source_url: https://keryx.cc/api/docs
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://keryx.cc/api/docs\nsources:\n- https://keryx.cc/api/docs\ndescription: 'Authentication: Two modes — x402-only: attach a valid payment-signature header (x402 v2 format). No key needed. Key + x402: mint\n  an API key at /api/keys (SIWE wallet required), then attach both Authorization: Bearer kx_live_… and payment-signature. Key adds identity, rate-limit,\n  and usage metering — it does NOT waive the payment requirement. No free compute.'\nschemes:\n- type: apiKey\n  name: payment-signature\n  evidence: 'x402-only: attach a valid payment-signature header (x402 v2 format). No key needed.'\n  location: header\n  header: payment-signature\n- type: http-bearer\n  name: Authorization\n  evidence: 'Key + x402: mint an API key at /api/keys (SIWE wallet required), then attach both Authorization: Bearer kx_live_… and payment-signature.'\n  location: header\n  header: Authorization\n\
  \  how_to_obtain: Mint an API key at /api/keys (SIWE wallet required).\ndocs: https://keryx.cc/api/docs\n"
source_yaml_url: https://artifacts.apis.io/keryx-cc/authentication/keryx-cc-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Research
- Platform
- Open Source
- Blockchain
---
