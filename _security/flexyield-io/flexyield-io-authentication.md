---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flexyield-io-agents-api-openapi.yml
  format: yaml
  label: flexyield-io Agents API
  slug: flexyield-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-agents-api-openapi.yml
- filename: flexyield-io-data-api-openapi.yml
  format: yaml
  label: flexyield-io Data API
  slug: flexyield-io-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-data-api-openapi.yml
- filename: flexyield-io-keys-api-openapi.yml
  format: yaml
  label: flexyield-io Keys API
  slug: flexyield-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-keys-api-openapi.yml
- filename: flexyield-io-rpc-api-openapi.yml
  format: yaml
  label: flexyield-io Rpc API
  slug: flexyield-io-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-rpc-api-openapi.yml
- filename: flexyield-io-statements-api-openapi.yml
  format: yaml
  label: flexyield-io Statements API
  slug: flexyield-io-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-statements-api-openapi.yml
- filename: flexyield-io-toolbox-api-openapi.yml
  format: yaml
  label: flexyield-io Toolbox API
  slug: flexyield-io-toolbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-toolbox-api-openapi.yml
- filename: flexyield-io-x402-api-openapi.yml
  format: yaml
  label: flexyield-io X402 API
  slug: flexyield-io-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-x402-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Flexyield Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: flexyield-io secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: flexyield-io
provider_slug: flexyield-io
scheme_count: 2
schemes:
- description: Your FlexYield API key (fy_…). Free tier at https://flexyield.io/registration/new
  name: bearer
  scheme: bearer
  sources:
  - openapi/flexyield-io-openapi.json
  type: http
- description: 'x402 lane: the one-time credential (fyx_…) returned by POST https://flexyield.io/x402/redeem after a payment against the menu at https://flexyield.io/x402 (base); the redeem needs an EIP-191 signature by the paying wallet — the tx hash alone is public and is not a credential'
  in: header
  name: x402
  parameter: X-PAYMENT
  sources:
  - openapi/flexyield-io-openapi.json
  type: apiKey
slug: flexyield-io-authentication
source_filename: flexyield-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/flexyield-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Your FlexYield API key (fy_…). Free tier at https://flexyield.io/registration/new\n  sources:\n  - openapi/flexyield-io-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: 'x402 lane: the one-time credential (fyx_…) returned by POST https://flexyield.io/x402/redeem\n    after a payment against the menu at https://flexyield.io/x402 (base); the redeem needs an\n    EIP-191 signature by the paying wallet — the tx hash alone is public and is not a credential'\n  sources:\n  - openapi/flexyield-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flexyield-io/authentication/flexyield-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Blockchain
- API Gateway
- Unified Billing
- Multi-Chain
- Free Tier
---
