---
api_key_in:
- header
api_specs:
- filename: hour-one-general-api-openapi.yml
  format: yaml
  label: Hour One general API
  slug: hour-one-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hour-one/refs/heads/main/openapi/hour-one-general-api-openapi.yml
- filename: hour-one-keys-api-openapi.yml
  format: yaml
  label: Hour One keys API
  slug: hour-one-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hour-one/refs/heads/main/openapi/hour-one-keys-api-openapi.yml
- filename: hour-one-playground-api-openapi.yml
  format: yaml
  label: Hour One playground API
  slug: hour-one-playground-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hour-one/refs/heads/main/openapi/hour-one-playground-api-openapi.yml
- filename: hour-one-videos-api-openapi.yml
  format: yaml
  label: Hour One videos API
  slug: hour-one-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hour-one/refs/heads/main/openapi/hour-one-videos-api-openapi.yml
- filename: hour-one-voice-preview-api-openapi.yml
  format: yaml
  label: Hour One voice-preview API
  slug: hour-one-voice-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hour-one/refs/heads/main/openapi/hour-one-voice-preview-api-openapi.yml
- filename: hour-one-webhook-api-openapi.yml
  format: yaml
  label: Hour One webhook API
  slug: hour-one-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hour-one/refs/heads/main/openapi/hour-one-webhook-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hour One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hour One secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hour One
provider_slug: hour-one
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: api-key
  sources:
  - openapi/hour-one-openapi.json
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/hour-one-openapi.json
  type: http
slug: hour-one-authentication
source_filename: hour-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hour-one-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/hour-one-openapi.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hour-one-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hour-one/refs/heads/main/authentication/hour-one-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Video
- Generative AI
- AI Video
- Media
- Text to Video
- Avatars
- Content Creation
---
