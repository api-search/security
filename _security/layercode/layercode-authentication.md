---
api_key_in: []
api_specs:
- filename: layercode-openapi.yml
  format: yaml
  label: Layercode Agents API
  slug: layercode-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/openapi/layercode-openapi.yml
- filename: layercode-openapi.yml
  format: yaml
  label: Layercode Sessions API
  slug: layercode-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/openapi/layercode-openapi.yml
- filename: layercode-asyncapi.yml
  format: yaml
  label: Layercode Realtime Voice API
  slug: layercode-realtime-voice-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/asyncapi/layercode-asyncapi.yml
- filename: layercode-asyncapi.yml
  format: yaml
  label: Layercode Webhooks API
  slug: layercode-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/asyncapi/layercode-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Layercode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Layercode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Layercode
provider_slug: layercode
scheme_count: 1
schemes:
- description: Org-scoped Layercode API key passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/layercode-openapi.yml
  type: http
slug: layercode-authentication
source_filename: layercode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/layercode-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Org-scoped Layercode API key passed as a Bearer token.\n  sources:\n  - openapi/layercode-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/authentication/layercode-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice
- Voice Agents
- Realtime
- Low Latency
---
