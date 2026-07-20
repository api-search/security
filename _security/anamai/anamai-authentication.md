---
api_key_in: []
api_specs:
- filename: anamai-openapi-original.json
  format: json
  label: Anam AI API
  slug: anam-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-openapi-original.json
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
