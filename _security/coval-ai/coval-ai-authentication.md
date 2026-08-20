---
api_key_in:
- header
api_specs:
- filename: coval-ai-agents-api-openapi.yml
  format: yaml
  label: Coval Agents API
  slug: coval-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-agents-api-openapi.yml
- filename: coval-ai-conversations-api-openapi.yml
  format: yaml
  label: Coval Conversations API
  slug: coval-ai-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-conversations-api-openapi.yml
- filename: coval-ai-metrics-api-openapi.yml
  format: yaml
  label: Coval Metrics API
  slug: coval-ai-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-metrics-api-openapi.yml
- filename: coval-ai-mutations-api-openapi.yml
  format: yaml
  label: Coval Mutations API
  slug: coval-ai-mutations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-mutations-api-openapi.yml
- filename: coval-ai-personas-api-openapi.yml
  format: yaml
  label: Coval Personas API
  slug: coval-ai-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-personas-api-openapi.yml
- filename: coval-ai-reports-api-openapi.yml
  format: yaml
  label: Coval Reports API
  slug: coval-ai-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-reports-api-openapi.yml
- filename: coval-ai-run-templates-api-openapi.yml
  format: yaml
  label: Coval Run Templates API
  slug: coval-ai-run-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-run-templates-api-openapi.yml
- filename: coval-ai-runs-api-openapi.yml
  format: yaml
  label: Coval Runs API
  slug: coval-ai-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-runs-api-openapi.yml
- filename: coval-ai-scheduled-runs-api-openapi.yml
  format: yaml
  label: Coval Scheduled Runs API
  slug: coval-ai-scheduled-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-scheduled-runs-api-openapi.yml
- filename: coval-ai-simulations-api-openapi.yml
  format: yaml
  label: Coval Simulations API
  slug: coval-ai-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-simulations-api-openapi.yml
- filename: coval-ai-test-cases-api-openapi.yml
  format: yaml
  label: Coval Test Cases API
  slug: coval-ai-test-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-test-cases-api-openapi.yml
- filename: coval-ai-test-sets-api-openapi.yml
  format: yaml
  label: Coval Test Sets API
  slug: coval-ai-test-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-test-sets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coval Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coval secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coval
provider_slug: coval-ai
scheme_count: 1
schemes:
- description: Organization API key for authentication.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/coval-ai-openapi.yml
  type: apiKey
slug: coval-ai-authentication
source_filename: coval-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coval-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Organization API key for authentication.\n  sources:\n  - openapi/coval-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/authentication/coval-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Agents
- Voice AI
- Simulation
- Evaluation
- Testing
---
