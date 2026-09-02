---
api_key_in: []
api_specs:
- filename: reka-chat-api-openapi.yml
  format: yaml
  label: Reka Chat API
  slug: reka-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-chat-api-openapi.yml
- filename: reka-clips-api-openapi.yml
  format: yaml
  label: Reka Clips API
  slug: reka-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-clips-api-openapi.yml
- filename: reka-models-api-openapi.yml
  format: yaml
  label: Reka Models API
  slug: reka-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-models-api-openapi.yml
- filename: reka-qa-api-openapi.yml
  format: yaml
  label: Reka QA API
  slug: reka-qa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-qa-api-openapi.yml
- filename: reka-research-api-openapi.yml
  format: yaml
  label: Reka Research API
  slug: reka-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-research-api-openapi.yml
- filename: reka-search-api-openapi.yml
  format: yaml
  label: Reka Search API
  slug: reka-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-search-api-openapi.yml
- filename: reka-speech-api-openapi.yml
  format: yaml
  label: Reka Speech API
  slug: reka-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-speech-api-openapi.yml
- filename: reka-videogroups-api-openapi.yml
  format: yaml
  label: Reka VideoGroups API
  slug: reka-videogroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-videogroups-api-openapi.yml
- filename: reka-videos-api-openapi.yml
  format: yaml
  label: Reka Videos API
  slug: reka-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reka secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reka
provider_slug: reka
scheme_count: 1
schemes:
- bearerFormat: REKA_API_KEY
  description: 'Bearer token issued from the Reka Platform dashboard. Pass as

    `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/reka-openapi.yml
  type: http
slug: reka-authentication
source_filename: reka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reka-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: REKA_API_KEY\n  description: |-\n    Bearer token issued from the Reka Platform dashboard. Pass as\n    `Authorization: Bearer [example key]`.\n  sources:\n  - openapi/reka-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/authentication/reka-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Multi-Modal
- Large Language Models
- Vision
- Speech
- Foundation Models
- OpenAI-Compatible
- SDK
- Enterprise
- On-Premises
---
