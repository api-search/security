---
api_key_in:
- header
api_specs:
- filename: reasonblocks-openapi-original.json
  format: json
  label: ReasonBlocks REST API
  slug: reasonblocks-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-openapi-original.json
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
