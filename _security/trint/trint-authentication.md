---
api_key_in: []
api_specs:
- filename: trint-openapi.yml
  format: yaml
  label: Trint Upload and Transcribe API
  slug: trint-upload-transcribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Transcripts and Files API
  slug: trint-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Export API
  slug: trint-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Translations API
  slug: trint-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Realtime Transcription API
  slug: trint-realtime-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Webhooks API
  slug: trint-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trint secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trint
provider_slug: trint
scheme_count: 2
schemes:
- name: basicAuth
  notes: Recommended. HTTP Basic using the API Key ID as username and API Key Secret as password, Base64-encoded in the Authorization header.
  scheme: basic
  sources:
  - openapi/trint-openapi.yml
  type: http
- in: header
  keyName: api-key
  name: legacyApiKey
  notes: Legacy authentication - the legacy key value is sent in the api-key header.
  sources:
  - openapi/trint-openapi.yml
  type: apiKey
slug: trint-authentication
source_filename: trint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trint-openapi.yml\nsummary:\n  types:\n  - http\n  - apiKey\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/trint-openapi.yml\n  notes: >-\n    Recommended. HTTP Basic using the API Key ID as username and API Key Secret\n    as password, Base64-encoded in the Authorization header.\n- name: legacyApiKey\n  type: apiKey\n  in: header\n  keyName: api-key\n  sources:\n  - openapi/trint-openapi.yml\n  notes: Legacy authentication - the legacy key value is sent in the api-key header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/authentication/trint-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Audio Transcription
- Transcription
- Speech-to-Text
- Media
- Journalism
- AI
- Captions
---
