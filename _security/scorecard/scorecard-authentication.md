---
api_key_in: []
api_specs:
- filename: scorecard-metrics-api-openapi.yml
  format: yaml
  label: Scorecard Metrics API
  slug: scorecard-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-metrics-api-openapi.yml
- filename: scorecard-projects-api-openapi.yml
  format: yaml
  label: Scorecard Projects API
  slug: scorecard-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-projects-api-openapi.yml
- filename: scorecard-records-api-openapi.yml
  format: yaml
  label: Scorecard Records API
  slug: scorecard-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-records-api-openapi.yml
- filename: scorecard-runs-api-openapi.yml
  format: yaml
  label: Scorecard Runs API
  slug: scorecard-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-runs-api-openapi.yml
- filename: scorecard-systems-api-openapi.yml
  format: yaml
  label: Scorecard Systems API
  slug: scorecard-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-systems-api-openapi.yml
- filename: scorecard-testcases-api-openapi.yml
  format: yaml
  label: Scorecard Testcases API
  slug: scorecard-testcases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-testcases-api-openapi.yml
- filename: scorecard-testsets-api-openapi.yml
  format: yaml
  label: Scorecard Testsets API
  slug: scorecard-testsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-testsets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scorecard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scorecard secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scorecard
provider_slug: scorecard
scheme_count: 1
schemes:
- bearerFormat: starts with ak_
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/scorecard-openapi-original.yml
  type: http
slug: scorecard-authentication
source_filename: scorecard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/scorecard-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: starts with ak_\n  sources:\n  - openapi/scorecard-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/authentication/scorecard-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Agents
- Evaluation
- Testing
- LLM
- Observability
- Simulation
- Developer Tools
- MCP
---
