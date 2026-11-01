---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Daishi Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: daishi-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: daishi-ai
provider_slug: daishi-ai
scheme_count: 2
schemes:
- description: Send token as Bearer header
  scheme: bearer
  type: http
- description: Alternative header for token
  in: header
  name: x-api-key
  type: apiKey
slug: daishi-ai-authentication
source_filename: daishi-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://daishi.ai/docs/developer/authentication?format=md\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Send token as Bearer header\"\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: \"Alternative header for token\"\n"
source_yaml_url: https://artifacts.apis.io/daishi-ai/authentication/daishi-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Agents
- Platform
- Evaluation
- Simulation
- Marketplace
- Benchmark
---
