---
api_key_in:
- header
api_specs:
- filename: lmnt-speech-openapi.yml
  format: yaml
  label: LMNT Speech API
  slug: lmnt-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lmnt/refs/heads/main/openapi/lmnt-speech-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lmnt Authentication
name_suffix: Authentication
oauth_flows: []
overview: LMNT secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LMNT
provider_slug: lmnt
scheme_count: 1
schemes:
- description: API key obtained from the LMNT dashboard at https://app.lmnt.com
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/lmnt-speech-openapi.yml
  type: apiKey
slug: lmnt-authentication
source_filename: lmnt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lmnt-speech-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key obtained from the LMNT dashboard at https://app.lmnt.com\n  sources:\n  - openapi/lmnt-speech-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lmnt/refs/heads/main/authentication/lmnt-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- text-to-speech
- voice synthesis
- voice cloning
- audio streaming
- conversational AI
- low latency
- real-time audio
---
