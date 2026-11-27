---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: palmyr-ai-cards-api-openapi.yml
  format: yaml
  label: Palmyr Cards API
  slug: palmyr-ai-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-cards-api-openapi.yml
- filename: palmyr-ai-communications-api-openapi.yml
  format: yaml
  label: Palmyr Communications API
  slug: palmyr-ai-communications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-communications-api-openapi.yml
- filename: palmyr-ai-compute-api-openapi.yml
  format: yaml
  label: Palmyr Compute API
  slug: palmyr-ai-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-compute-api-openapi.yml
- filename: palmyr-ai-domains-api-openapi.yml
  format: yaml
  label: Palmyr Domains API
  slug: palmyr-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-domains-api-openapi.yml
- filename: palmyr-ai-email-api-openapi.yml
  format: yaml
  label: Palmyr Email API
  slug: palmyr-ai-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-email-api-openapi.yml
- filename: palmyr-ai-free-api-openapi.yml
  format: yaml
  label: Palmyr Free API
  slug: palmyr-ai-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-free-api-openapi.yml
- filename: palmyr-ai-orchestration-api-openapi.yml
  format: yaml
  label: Palmyr Orchestration API
  slug: palmyr-ai-orchestration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-orchestration-api-openapi.yml
- filename: palmyr-ai-phone-api-openapi.yml
  format: yaml
  label: Palmyr Phone API
  slug: palmyr-ai-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-phone-api-openapi.yml
- filename: palmyr-ai-social-api-openapi.yml
  format: yaml
  label: Palmyr Social API
  slug: palmyr-ai-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/palmyr-ai/openapi/palmyr-ai-social-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Palmyr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Palmyr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Palmyr
provider_slug: palmyr-ai
scheme_count: 1
schemes:
- description: x402 payment payload (Solana or EVM USDC). See the 402 challenge response on any paid endpoint.
  in: header
  name: x402
  parameter: X-Payment
  sources:
  - openapi/palmyr-ai-openapi.json
  type: apiKey
slug: palmyr-ai-authentication
source_filename: palmyr-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/palmyr-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-Payment\n  description: x402 payment payload (Solana or EVM USDC). See the 402 challenge response on\n    any paid endpoint.\n  sources:\n  - openapi/palmyr-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/palmyr-ai/authentication/palmyr-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Infrastructure
- Autonomous Agents
- Payments
- USDC
---
