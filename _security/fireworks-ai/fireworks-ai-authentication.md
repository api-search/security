---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fireworks-ai-anthropic-messages-openapi-other-api-openapi.yml
  format: yaml
  label: Fireworks AI anthropic-messages.openapi_other API
  slug: fireworks-ai-anthropic-messages-openapi-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-anthropic-messages-openapi-other-api-openapi.yml
- filename: fireworks-ai-gateway-extra-openapi-gateway-api-openapi.yml
  format: yaml
  label: Fireworks AI gateway-extra.openapi_Gateway API
  slug: fireworks-ai-gateway-extra-openapi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-gateway-extra-openapi-gateway-api-openapi.yml
- filename: fireworks-ai-gateway-openapi-gateway-api-openapi.yml
  format: yaml
  label: Fireworks AI gateway.openapi_Gateway API
  slug: fireworks-ai-gateway-openapi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-gateway-openapi-gateway-api-openapi.yml
- filename: fireworks-ai-responses-openapi-other-api-openapi.yml
  format: yaml
  label: Fireworks AI responses.openapi_other API
  slug: fireworks-ai-responses-openapi-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-responses-openapi-other-api-openapi.yml
- filename: fireworks-ai-text-completion-openapi-other-api-openapi.yml
  format: yaml
  label: Fireworks AI text-completion.openapi_other API
  slug: fireworks-ai-text-completion-openapi-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-text-completion-openapi-other-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fireworks Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fireworks AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fireworks AI
provider_slug: fireworks-ai
scheme_count: 1
schemes:
- bearerFormat: API_KEY
  description: 'Bearer authentication using your Fireworks API key. Format: Bearer <API_KEY>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fireworks-ai-anthropic-messages-openapi.json
  - openapi/fireworks-ai-gateway-openapi.yml
  - openapi/fireworks-ai-merged-openapi.yml
  - openapi/fireworks-ai-responses-openapi.yml
  - openapi/fireworks-ai-text-completion-openapi.yml
  type: http
slug: fireworks-ai-authentication
source_filename: fireworks-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fireworks-ai-anthropic-messages-openapi.json, openapi/fireworks-ai-gateway-openapi.yml,\n  openapi/fireworks-ai-merged-openapi.yml, openapi/fireworks-ai-responses-openapi.yml, openapi/fireworks-ai-text-completion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API_KEY\n  description: 'Bearer authentication using your Fireworks API key. Format: Bearer <API_KEY>'\n  sources:\n  - openapi/fireworks-ai-anthropic-messages-openapi.json\n  - openapi/fireworks-ai-gateway-openapi.yml\n  - openapi/fireworks-ai-merged-openapi.yml\n  - openapi/fireworks-ai-responses-openapi.yml\n  - openapi/fireworks-ai-text-completion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/authentication/fireworks-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Inference
- Multi-Modal
- Fine-Tuning
- GPU
---
