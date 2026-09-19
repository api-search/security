---
anonymous_access: false
api_key_in: []
api_specs:
- filename: actionpower-image-api-openapi.yml
  format: yaml
  label: Actionpower Image API
  slug: actionpower-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/openapi/actionpower-image-api-openapi.yml
- filename: actionpower-nlp-api-openapi.yml
  format: yaml
  label: Actionpower NLP API
  slug: actionpower-nlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/openapi/actionpower-nlp-api-openapi.yml
- filename: actionpower-stt-api-openapi.yml
  format: yaml
  label: Actionpower STT API
  slug: actionpower-stt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/openapi/actionpower-stt-api-openapi.yml
- filename: actionpower-tts-api-openapi.yml
  format: yaml
  label: Actionpower TTS API
  slug: actionpower-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/openapi/actionpower-tts-api-openapi.yml
- filename: actionpower-video-api-openapi.yml
  format: yaml
  label: Actionpower Video API
  slug: actionpower-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/openapi/actionpower-video-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Actionpower Authentication
name_suffix: Authentication
oauth_flows: []
overview: Actionpower secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Actionpower
provider_slug: actionpower
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/actionpower-daglo-cloud-api-dev-openapi.yml
  - openapi/actionpower-daglo-cloud-api-openapi.yml
  type: http
slug: actionpower-authentication
source_filename: actionpower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/actionpower-daglo-cloud-api-dev-openapi.yml, openapi/actionpower-daglo-cloud-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/actionpower-daglo-cloud-api-dev-openapi.yml\n  - openapi/actionpower-daglo-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/authentication/actionpower-authentication.yml
summary_line: http · 1 scheme
tags:
- Speech Recognition
- Speech-to-Text
- Text-to-Speech
- Natural Language Processing
- Artificial Intelligence
- Transcription
- Voice
- Meeting Intelligence
- gRPC
- South Korea
---
