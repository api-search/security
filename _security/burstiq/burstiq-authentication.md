---
api_key_in: []
api_specs:
- filename: burstiq-lifegraph-openapi-original.json
  format: json
  label: BurstIQ LifeGraph API
  slug: burstiq-lifegraph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burstiq/refs/heads/main/openapi/burstiq-lifegraph-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Burstiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: BurstIQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BurstIQ
provider_slug: burstiq
scheme_count: 1
schemes:
- applied: runtime-enforced (not declared in OpenAPI)
  bearer_format: JWT
  evidence: 'HTTP 401 WWW-Authenticate: Bearer on https://api.burstiq.com'
  name: bearerAuth
  scheme: bearer
  sources:
  - live-probe
  type: http
slug: burstiq-authentication
source_filename: burstiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: live probe of https://api.burstiq.com (HTTP 401 + WWW-Authenticate header)\nnote: >-\n  The published LifeGraph OpenAPI (openapi/burstiq-lifegraph-openapi-original.json)\n  declares no components.securitySchemes, but the live API enforces bearer-token\n  authentication: unauthenticated requests to https://api.burstiq.com return\n  HTTP 401 with `WWW-Authenticate: Bearer`. This profile records the observed\n  runtime auth model; the spec itself omits the scheme.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  evidence: 'HTTP 401 WWW-Authenticate: Bearer on https://api.burstiq.com'\n  applied: runtime-enforced (not declared in OpenAPI)\n  sources:\n  - live-probe\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burstiq/refs/heads/main/authentication/burstiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Health
- Data
- Blockchain
- Knowledge Graph
- Consent
- Agentic AI
---
