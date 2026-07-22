---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Optimizerai Authentication
name_suffix: Authentication
oauth_flows: []
overview: OptimizerAI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OptimizerAI
provider_slug: optimizerai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  scope: project
  sources:
  - https://docs.optimizerai.xyz/api/pricing
  transport: https
  type: apiKey
slug: optimizerai-authentication
source_filename: optimizerai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.optimizerai.xyz/api/pricing\ndocs: https://docs.optimizerai.xyz/api/pricing\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    OptimizerAI authenticates each request with a project-specific API key sent\n    over an HTTPS header, per the published API Pricing & SLA documentation.\n    Keys are scoped to a project/contract; there is no public OAuth or OpenID\n    Connect surface. Exact header name and key issuance flow are not published\n    on the public docs and are provisioned as part of a commercial contract.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  scope: project\n  transport: https\n  sources:\n  - https://docs.optimizerai.xyz/api/pricing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimizerai/refs/heads/main/authentication/optimizerai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Sound Effects
- Audio
- Generative AI
- Text to Audio
- Game Development
- Media and Entertainment
- Machine Learning
- Creator Tools
---
