---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Simudyne Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simudyne secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Simudyne
provider_slug: simudyne
scheme_count: 1
schemes:
- description: The Pulse REST API and Python SDK authenticate with a live API key (prefix "pk_live_"). The SDK reads it from the SIMUDYNE_API_KEY environment variable or accepts it directly via the PulseABM(api_key=...) constructor. Free-tier keys require no credit card; sign up at https://pulse.simudyne.com/auth/signin.
  env_var: SIMUDYNE_API_KEY
  in: header
  key_prefix: pk_live_
  name: PulseApiKey
  sdk_param: PulseABM(api_key="pk_live_...")
  type: apiKey
slug: simudyne-authentication
source_filename: simudyne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://pulse.simudyne.com/llms.txt + https://github.com/simudyne/pulse-sdk\ndocs: https://pulse.simudyne.com/docs\napi: Pulse synthetic market data API\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: PulseApiKey\n    type: apiKey\n    in: header\n    key_prefix: pk_live_\n    env_var: SIMUDYNE_API_KEY\n    sdk_param: PulseABM(api_key=\"pk_live_...\")\n    description: >-\n      The Pulse REST API and Python SDK authenticate with a live API key\n      (prefix \"pk_live_\"). The SDK reads it from the SIMUDYNE_API_KEY\n      environment variable or accepts it directly via the PulseABM(api_key=...)\n      constructor. Free-tier keys require no credit card; sign up at\n      https://pulse.simudyne.com/auth/signin.\nsignup: https://pulse.simudyne.com/auth/signin\nnotes: >-\n  No OpenAPI/Swagger document was discoverable at the common paths\n  (/openapi.json, /openapi.yaml, /redoc all\
  \ 404), so this profile is captured\n  from the published SDK and llms.txt rather than derived from a spec. No OAuth2\n  or OpenID Connect surface is documented — key-auth only, so no scopes/\n  artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simudyne/refs/heads/main/authentication/simudyne-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Simulation
- Agent-Based Modeling
- Synthetic Data
- Market Data
- Financial Services
- Machine Learning
- Developer SDK
---
