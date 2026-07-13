---
api_key_in: []
api_specs:
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Applications API
  slug: refuel-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Tasks API
  slug: refuel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Datasets API
  slug: refuel-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Labeling and Predict API
  slug: refuel-labeling-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Models API
  slug: refuel-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Refuel Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refuel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Refuel
provider_slug: refuel-ai
scheme_count: 1
schemes:
- description: 'Refuel API key supplied as a Bearer token in the Authorization header: Authorization: Bearer <YOUR_API_KEY>.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/refuel-ai-openapi.yml
  type: http
slug: refuel-ai-authentication
source_filename: refuel-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/refuel-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Refuel API key supplied as a Bearer token in the Authorization header: Authorization:\n    Bearer <YOUR_API_KEY>.'\n  sources:\n  - openapi/refuel-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/authentication/refuel-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Data Labeling
- Data Enrichment
- Autolabel
---
