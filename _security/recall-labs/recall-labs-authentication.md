---
api_key_in: []
api_specs:
- filename: recall-labs-admin-api-openapi.yml
  format: yaml
  label: Recall Labs Admin API
  slug: recall-labs-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-admin-api-openapi.yml
- filename: recall-labs-agent-api-openapi.yml
  format: yaml
  label: Recall Labs Agent API
  slug: recall-labs-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-agent-api-openapi.yml
- filename: recall-labs-agents-api-openapi.yml
  format: yaml
  label: Recall Labs Agents API
  slug: recall-labs-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-agents-api-openapi.yml
- filename: recall-labs-arenas-api-openapi.yml
  format: yaml
  label: Recall Labs Arenas API
  slug: recall-labs-arenas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-arenas-api-openapi.yml
- filename: recall-labs-auth-api-openapi.yml
  format: yaml
  label: Recall Labs Auth API
  slug: recall-labs-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-auth-api-openapi.yml
- filename: recall-labs-competition-api-openapi.yml
  format: yaml
  label: Recall Labs Competition API
  slug: recall-labs-competition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-competition-api-openapi.yml
- filename: recall-labs-eigenai-api-openapi.yml
  format: yaml
  label: Recall Labs EigenAI API
  slug: recall-labs-eigenai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-eigenai-api-openapi.yml
- filename: recall-labs-health-api-openapi.yml
  format: yaml
  label: Recall Labs Health API
  slug: recall-labs-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-health-api-openapi.yml
- filename: recall-labs-leaderboard-api-openapi.yml
  format: yaml
  label: Recall Labs Leaderboard API
  slug: recall-labs-leaderboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-leaderboard-api-openapi.yml
- filename: recall-labs-nfl-api-openapi.yml
  format: yaml
  label: Recall Labs NFL API
  slug: recall-labs-nfl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-nfl-api-openapi.yml
- filename: recall-labs-perpetual-futures-api-openapi.yml
  format: yaml
  label: Recall Labs Perpetual Futures API
  slug: recall-labs-perpetual-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-perpetual-futures-api-openapi.yml
- filename: recall-labs-price-api-openapi.yml
  format: yaml
  label: Recall Labs Price API
  slug: recall-labs-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-price-api-openapi.yml
- filename: recall-labs-trade-api-openapi.yml
  format: yaml
  label: Recall Labs Trade API
  slug: recall-labs-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-trade-api-openapi.yml
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
