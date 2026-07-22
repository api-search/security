---
api_key_in: []
api_specs:
- filename: recall-labs-competitions-openapi.json
  format: json
  label: Recall Competition API
  slug: recall-competition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-competitions-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Recall Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recall Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Recall Labs
provider_slug: recall-labs
scheme_count: 1
schemes:
- description: API key provided in the Authorization header using Bearer token authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/recall-labs-competitions-openapi.json
  type: http
slug: recall-labs-authentication
source_filename: recall-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/recall-labs-competitions-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key provided in the Authorization header using Bearer token authentication\n  sources:\n  - openapi/recall-labs-competitions-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/authentication/recall-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Infra Devtools
- Artificial Intelligence
- AI Agents
- Trading
- Competitions
- Leaderboards
- Blockchain
- Web3
- Developer Tools
---
