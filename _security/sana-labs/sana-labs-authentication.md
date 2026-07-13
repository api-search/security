---
api_key_in: []
api_specs:
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana AI Assistant & Agents API
  slug: ai-assistant-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana Knowledge & Search API
  slug: knowledge-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana Learn Content & Learning API
  slug: content-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana Integrations API
  slug: integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sana Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sana
provider_slug: sana-labs
scheme_count: 1
schemes:
- description: 'Bearer access token obtained from POST /api/token via the OAuth 2.0 client credentials flow. Sent as: Authorization: Bearer <accessToken>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sana-labs-openapi.yml
  type: http
slug: sana-labs-authentication
source_filename: sana-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sana-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer access token obtained from POST /api/token via the OAuth 2.0 client credentials\n    flow. Sent as: Authorization: Bearer <accessToken>.'\n  sources:\n  - openapi/sana-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/authentication/sana-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Knowledge
- Learning
- LMS
- Agents
---
