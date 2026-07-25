---
api_key_in: []
api_specs:
- filename: kataai-auth-api-openapi.yml
  format: yaml
  label: Kata.ai Auth API
  slug: kataai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-auth-api-openapi.yml
- filename: kataai-bots-api-openapi.yml
  format: yaml
  label: Kata.ai Bots API
  slug: kataai-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-bots-api-openapi.yml
- filename: kataai-channels-api-openapi.yml
  format: yaml
  label: Kata.ai Channels API
  slug: kataai-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-channels-api-openapi.yml
- filename: kataai-deployments-api-openapi.yml
  format: yaml
  label: Kata.ai Deployments API
  slug: kataai-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-deployments-api-openapi.yml
- filename: kataai-environments-api-openapi.yml
  format: yaml
  label: Kata.ai Environments API
  slug: kataai-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-environments-api-openapi.yml
- filename: kataai-nlu-api-openapi.yml
  format: yaml
  label: Kata.ai NLU API
  slug: kataai-nlu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-nlu-api-openapi.yml
- filename: kataai-prediction-api-openapi.yml
  format: yaml
  label: Kata.ai Prediction API
  slug: kataai-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-prediction-api-openapi.yml
- filename: kataai-projects-api-openapi.yml
  format: yaml
  label: Kata.ai Projects API
  slug: kataai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-projects-api-openapi.yml
- filename: kataai-teams-api-openapi.yml
  format: yaml
  label: Kata.ai Teams API
  slug: kataai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kataai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kata.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kata.ai
provider_slug: kataai
scheme_count: 1
schemes:
- description: 'Bearer token in the Authorization header (Authorization: Bearer <token>). The token may alternatively be supplied as a ?token= query string parameter.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kataai-platform-openapi.yml
  type: http
slug: kataai-authentication
source_filename: kataai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kataai-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token in the Authorization header (Authorization: Bearer <token>). The\n    token may alternatively be supplied as a ?token= query string parameter.'\n  sources:\n  - openapi/kataai-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/authentication/kataai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conversational AI
- Chatbots
- AI Agents
- Natural Language Understanding
- NLU
- Customer Experience
- Messaging
- Indonesia
- Bots
---
