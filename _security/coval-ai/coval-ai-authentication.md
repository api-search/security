---
api_key_in:
- header
api_specs:
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Simulations & Runs API
  slug: simulations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Scenarios & Personas API
  slug: scenarios
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Metrics & Scorers API
  slug: metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Conversations & Observability API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
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
- AI
- Agents
- Voice AI
- Simulation
- Evaluation
- Testing
---
