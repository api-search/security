---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mediacaption.v1.yaml
  format: yaml
  label: Media Caption Public API
  slug: media-caption-public-api
  spec_type: OpenAPI
  url: https://www.mediacaption.io/docs/openapi/mediacaption.v1.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mediacaption Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: MediaCaption API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MediaCaption API
provider_slug: mediacaption-api
scheme_count: 2
schemes:
- bearerFormat: Media Caption API key
  description: 'Use `Authorization: Bearer mc_live_xxx`.'
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/mediacaption-api-openapi.yaml
  - https://www.mediacaption.io/docs/authentication
  type: http
- description: Alternative API key header.
  in: header
  name: headerApiKey
  parameter: X-API-Key
  sources:
  - openapi/mediacaption-api-openapi.yaml
  - https://www.mediacaption.io/docs/authentication
  type: apiKey
slug: mediacaption-api-authentication
source_filename: mediacaption-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/mediacaption-api-openapi.yaml + https://www.mediacaption.io/docs/authentication\ndocs: https://www.mediacaption.io/docs/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nkey_format: mc_live_ prefix; live keys only — no test-mode key prefix is published\nkey_management: Keys are created in the platform dashboard and shown once at creation.\nprecedence: When both headers are present, bearer authentication takes precedence.\nfailure_modes:\n  - code: missing_api_key\n    status: 401\n    when: no key is sent\n  - code: invalid_api_key\n    status: 401\n    when: malformed, unknown, or revoked keys\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: Media Caption API key\n  description: 'Use `Authorization: Bearer mc_live_xxx`.'\n  sources:\n  - openapi/mediacaption-api-openapi.yaml\n  - https://www.mediacaption.io/docs/authentication\n- name: headerApiKey\n\
  \  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Alternative API key header.\n  sources:\n  - openapi/mediacaption-api-openapi.yaml\n  - https://www.mediacaption.io/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediacaption-api/refs/heads/main/authentication/mediacaption-api-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- YouTube
- Transcription
- Captions
- Subtitles
- Video
- REST
- OpenAPI
- Webhook
- Speech-to-Text
- Media
- Developer Tools
---
