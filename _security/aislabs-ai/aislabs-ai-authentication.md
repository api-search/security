---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aislabs Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: aislabs-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: aislabs-ai
provider_slug: aislabs-ai
scheme_count: 2
schemes:
- description: x402 v1 payment payload (USDC on Base).
  in: header
  name: X-PAYMENT
  type: apiKey
- description: AIS Gateway key (ais_k_...), scoped per building.
  scheme: bearer
  type: http
slug: aislabs-ai-authentication
source_filename: aislabs-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://aislabs.ai/api-docs\nschemes:\n  - type: apiKey\n    in: header\n    name: X-PAYMENT\n    description: \"x402 v1 payment payload (USDC on Base).\"\n  - type: http\n    scheme: bearer\n    description: \"AIS Gateway key (ais_k_...), scoped per building.\"\n"
source_yaml_url: https://artifacts.apis.io/aislabs-ai/authentication/aislabs-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Tools
- Briefs
- Security
- Data
---
