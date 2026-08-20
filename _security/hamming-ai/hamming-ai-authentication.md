---
api_key_in: []
api_specs:
- filename: hamming-ai-datasets-api-openapi.yml
  format: yaml
  label: Hamming AI Datasets API
  slug: hamming-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-datasets-api-openapi.yml
- filename: hamming-ai-experiments-api-openapi.yml
  format: yaml
  label: Hamming AI Experiments API
  slug: hamming-ai-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-experiments-api-openapi.yml
- filename: hamming-ai-monitoring-api-openapi.yml
  format: yaml
  label: Hamming AI Monitoring API
  slug: hamming-ai-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-monitoring-api-openapi.yml
- filename: hamming-ai-prompts-api-openapi.yml
  format: yaml
  label: Hamming AI Prompts API
  slug: hamming-ai-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-prompts-api-openapi.yml
- filename: hamming-ai-scoring-api-openapi.yml
  format: yaml
  label: Hamming AI Scoring API
  slug: hamming-ai-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-scoring-api-openapi.yml
- filename: hamming-ai-voice-testing-api-openapi.yml
  format: yaml
  label: Hamming AI Voice Testing API
  slug: hamming-ai-voice-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-voice-testing-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hamming Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hamming AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hamming AI
provider_slug: hamming-ai
scheme_count: 1
schemes:
- description: A Hamming API key passed as a Bearer token in the Authorization header. Create a key at hamming.ai/settings.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hamming-ai-openapi.yml
  type: http
slug: hamming-ai-authentication
source_filename: hamming-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hamming-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A Hamming API key passed as a Bearer token in the Authorization header. Create\n    a key at hamming.ai/settings.\n  sources:\n  - openapi/hamming-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/authentication/hamming-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Voice Agents
- LLM
- Testing
- Evaluation
- Observability
---
