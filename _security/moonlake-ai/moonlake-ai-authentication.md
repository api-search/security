---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Moonlake Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoonLake AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MoonLake AI
provider_slug: moonlake-ai
scheme_count: 1
schemes:
- applies_to:
  - POST https://app.moonlakeai.com/api/jobs/
  bearerFormat: api_key
  description: 'API key supplied as an HTTP Bearer token, e.g. Authorization: Bearer {api_key}. Documented in the code sample on the Moonlake enterprise page and confirmed by the live 401 "Missing API key" response.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://moonlakeai.com/
  type: http
slug: moonlake-ai-authentication
source_filename: moonlake-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://moonlakeai.com/\ndocs: https://moonlakeai.com/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The MoonLake AI Generation API authenticates requests with a Bearer API key\n    passed in the Authorization header. Requests without a key return HTTP 401\n    with body {\"error\":\"Missing API key\"} (verified against\n    https://app.moonlakeai.com/api/jobs/). API keys are issued to enterprise\n    customers; there is no public self-serve sign-up (access is via \"Book Demo\").\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: api_key\n  description: >-\n    API key supplied as an HTTP Bearer token, e.g.\n    Authorization: Bearer {api_key}. Documented in the code sample on the\n    Moonlake enterprise page and confirmed by the live 401 \"Missing API key\"\n    response.\n  sources:\n  - https://moonlakeai.com/\n  applies_to:\n  - POST https://app.moonlakeai.com/api/jobs/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonlake-ai/refs/heads/main/authentication/moonlake-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- World Models
- Simulation
- Embodied AI
- Robotics
- 3D Generation
- Digital Twins
- Synthetic Data
---
