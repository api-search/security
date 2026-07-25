---
api_key_in:
- header
api_specs:
- filename: reasonblocks-billing-api-openapi.yml
  format: yaml
  label: ReasonBlocks Billing API
  slug: reasonblocks-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-billing-api-openapi.yml
- filename: reasonblocks-codebase-findings-api-openapi.yml
  format: yaml
  label: ReasonBlocks Codebase Findings API
  slug: reasonblocks-codebase-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-codebase-findings-api-openapi.yml
- filename: reasonblocks-health-api-openapi.yml
  format: yaml
  label: ReasonBlocks Health API
  slug: reasonblocks-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-health-api-openapi.yml
- filename: reasonblocks-monitor-api-openapi.yml
  format: yaml
  label: ReasonBlocks monitor API
  slug: reasonblocks-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-monitor-api-openapi.yml
- filename: reasonblocks-monitor-telemetry-api-openapi.yml
  format: yaml
  label: ReasonBlocks Monitor Telemetry API
  slug: reasonblocks-monitor-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-monitor-telemetry-api-openapi.yml
- filename: reasonblocks-monitors-api-openapi.yml
  format: yaml
  label: ReasonBlocks Monitors API
  slug: reasonblocks-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-monitors-api-openapi.yml
- filename: reasonblocks-pattern-library-api-openapi.yml
  format: yaml
  label: ReasonBlocks Pattern Library API
  slug: reasonblocks-pattern-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-pattern-library-api-openapi.yml
- filename: reasonblocks-patterns-traces-api-openapi.yml
  format: yaml
  label: ReasonBlocks Patterns & Traces API
  slug: reasonblocks-patterns-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-patterns-traces-api-openapi.yml
- filename: reasonblocks-scoring-api-openapi.yml
  format: yaml
  label: ReasonBlocks Scoring API
  slug: reasonblocks-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-scoring-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Reasonblocks Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReasonBlocks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ReasonBlocks
provider_slug: reasonblocks
scheme_count: 1
schemes:
- bearer_prefixes:
  - rb_live_
  - rb_test_
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/reasonblocks-openapi-original.json
  type: http
slug: reasonblocks-authentication
source_filename: reasonblocks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/reasonblocks-openapi-original.json\ndocs: https://docs.reasonblocks.com/api-reference/rest-api/setup\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nnotes: >-\n  Every route requires Authorization: Bearer <api_key>. Three credential paths:\n  per-customer keys issued from the dashboard (scoped to org_id / optional project_id;\n  live keys start rb_live_, test keys rb_test_), static keys via the REASONBLOCKS_KEYS\n  env var (self-hosted/CI/dev, no org scope), and a Supabase JWT for the dashboard UI\n  only. The key's scope is the authoritative tenant identity — body org_id fields are\n  ignored. No OAuth2/OIDC surface; no scope model.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearer_prefixes:\n  - rb_live_\n  - rb_test_\n  sources:\n  - openapi/reasonblocks-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/authentication/reasonblocks-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Agents
- Agent Observability
- LLM
- Developer Tools
- Token Optimization
- Agent Steering
- Machine Learning
- Artificial Intelligence
- SDK
---
