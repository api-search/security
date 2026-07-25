---
api_key_in: []
api_specs:
- filename: anamai-avatars-api-openapi.yml
  format: yaml
  label: Anam.ai Avatars API
  slug: anamai-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-avatars-api-openapi.yml
- filename: anamai-engine-api-openapi.yml
  format: yaml
  label: Anam.ai Engine API
  slug: anamai-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-engine-api-openapi.yml
- filename: anamai-knowledge-api-openapi.yml
  format: yaml
  label: Anam.ai Knowledge API
  slug: anamai-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-knowledge-api-openapi.yml
- filename: anamai-llms-api-openapi.yml
  format: yaml
  label: Anam.ai LLMs API
  slug: anamai-llms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-llms-api-openapi.yml
- filename: anamai-meetings-api-openapi.yml
  format: yaml
  label: Anam.ai Meetings API
  slug: anamai-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-meetings-api-openapi.yml
- filename: anamai-personas-api-openapi.yml
  format: yaml
  label: Anam.ai Personas API
  slug: anamai-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-personas-api-openapi.yml
- filename: anamai-sessions-api-openapi.yml
  format: yaml
  label: Anam.ai Sessions API
  slug: anamai-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-sessions-api-openapi.yml
- filename: anamai-share-links-api-openapi.yml
  format: yaml
  label: Anam.ai Share Links API
  slug: anamai-share-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-share-links-api-openapi.yml
- filename: anamai-tools-api-openapi.yml
  format: yaml
  label: Anam.ai Tools API
  slug: anamai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-tools-api-openapi.yml
- filename: anamai-voices-api-openapi.yml
  format: yaml
  label: Anam.ai Voices API
  slug: anamai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-voices-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anamai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anam.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anam.ai
provider_slug: anamai
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/anamai-openapi-original.json
  type: http
slug: anamai-authentication
source_filename: anamai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/anamai-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/anamai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/authentication/anamai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Avatars
- Conversational AI
- Real-Time Video
- WebRTC
- Digital Humans
- Generative AI
---
