---
anonymous_access: false
api_key_in: []
api_specs:
- filename: orkas-audio-api-openapi.yml
  format: yaml
  label: Orkas Audio API
  slug: orkas-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-audio-api-openapi.yml
- filename: orkas-images-api-openapi.yml
  format: yaml
  label: Orkas Images API
  slug: orkas-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-images-api-openapi.yml
- filename: orkas-openapi-json-api-openapi.yml
  format: yaml
  label: Orkas Openapi.json API
  slug: orkas-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-openapi-json-api-openapi.yml
- filename: orkas-search-api-openapi.yml
  format: yaml
  label: Orkas Search API
  slug: orkas-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-search-api-openapi.yml
- filename: orkas-videos-api-openapi.yml
  format: yaml
  label: Orkas Videos API
  slug: orkas-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-videos-api-openapi.yml
- filename: orkas-chat-completions-api-openapi.yml
  format: yaml
  label: Orkas Chat Completions API
  slug: orkas-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Orkas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orkas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orkas
provider_slug: orkas
scheme_count: 1
schemes:
- description: 'Orkas API key, sent as `Authorization: Bearer <key>`. Create one in the Orkas account settings.'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/orkas-openapi.yml
  type: http
slug: orkas-authentication
source_filename: orkas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: derived\nsource: openapi/orkas-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Orkas API key, sent as `Authorization: Bearer <key>`. Create one in the Orkas\n    account settings.'\n  sources:\n  - openapi/orkas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/authentication/orkas-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- API
- Chatbot
- Media
---
