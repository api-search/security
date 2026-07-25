---
api_key_in: []
api_specs:
- filename: anam-auth-api-openapi.yml
  format: yaml
  label: Anam Auth API
  slug: anam-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-auth-api-openapi.yml
- filename: anam-avatars-api-openapi.yml
  format: yaml
  label: Anam Avatars API
  slug: anam-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-avatars-api-openapi.yml
- filename: anam-knowledge-api-openapi.yml
  format: yaml
  label: Anam Knowledge API
  slug: anam-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-knowledge-api-openapi.yml
- filename: anam-llms-api-openapi.yml
  format: yaml
  label: Anam Llms API
  slug: anam-llms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-llms-api-openapi.yml
- filename: anam-personas-api-openapi.yml
  format: yaml
  label: Anam Personas API
  slug: anam-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-personas-api-openapi.yml
- filename: anam-sessions-api-openapi.yml
  format: yaml
  label: Anam Sessions API
  slug: anam-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-sessions-api-openapi.yml
- filename: anam-share-links-api-openapi.yml
  format: yaml
  label: Anam Share Links API
  slug: anam-share-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-share-links-api-openapi.yml
- filename: anam-tools-api-openapi.yml
  format: yaml
  label: Anam Tools API
  slug: anam-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-tools-api-openapi.yml
- filename: anam-voices-api-openapi.yml
  format: yaml
  label: Anam Voices API
  slug: anam-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-voices-api-openapi.yml
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
