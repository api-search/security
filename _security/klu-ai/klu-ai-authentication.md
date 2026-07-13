---
api_key_in: []
api_specs:
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Actions / Prompt API
  slug: klu-actions-prompt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Data / Feedback API
  slug: klu-data-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Models API
  slug: klu-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Sessions API
  slug: klu-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Apps / Workspaces API
  slug: klu-apps-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Klu Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Klu
provider_slug: klu-ai
scheme_count: 1
schemes:
- description: Klu API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/klu-ai-openapi.yml
  type: http
slug: klu-ai-authentication
source_filename: klu-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/klu-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Klu API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/klu-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/authentication/klu-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- LLM App Platform
- Prompt Engineering
- Evaluation
- Observability
---
