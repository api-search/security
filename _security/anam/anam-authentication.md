---
api_key_in: []
api_specs:
- filename: anam-openapi-original.json
  format: json
  label: Anam AI API
  slug: anam-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Anam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anam secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anam
provider_slug: anam
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/anam-openapi-original.json
  type: http
slug: anam-authentication
source_filename: anam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/anam-openapi-original.json + https://anam.ai/docs/api-reference/overview\ndocs: https://anam.ai/docs/api-reference/overview\nsummary:\n  types:\n  - http\n  scheme: bearer\n  model: >-\n    Two-step. A long-lived server API key (created in the Anam Lab dashboard) authenticates\n    all REST calls as `Authorization: Bearer <API_KEY>`. To open a client-side avatar session,\n    the API key is exchanged at POST /v1/auth/session-token for a short-lived signed session-token\n    JWT (valid ~1 hour) that the browser/mobile SDK uses to establish the WebRTC connection.\n  upload_alt: >-\n    Knowledge-document upload also accepts an X-Upload-Token header as an alternative to the\n    Bearer API key.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/anam-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/authentication/anam-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Avatars
- Conversational AI
- Video
- Real-Time
- Voice
- Agents
---
