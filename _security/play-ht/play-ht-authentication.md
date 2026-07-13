---
api_key_in:
- header
api_specs:
- filename: play-ht-openapi.yml
  format: yaml
  label: PlayHT API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/play-ht/refs/heads/main/openapi/play-ht-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Play Ht Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlayHT secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PlayHT
provider_slug: play-ht
scheme_count: 2
schemes:
- description: Secret API key generated in the PlayHT studio.
  in: header
  name: apiKey
  parameter: AUTHORIZATION
  sources:
  - openapi/play-ht-openapi.yml
  type: apiKey
- description: PlayHT user identifier paired with the API key.
  in: header
  name: userId
  parameter: X-USER-ID
  sources:
  - openapi/play-ht-openapi.yml
  type: apiKey
slug: play-ht-authentication
source_filename: play-ht-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/play-ht-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: AUTHORIZATION\n  description: Secret API key generated in the PlayHT studio.\n  sources:\n  - openapi/play-ht-openapi.yml\n- name: userId\n  type: apiKey\n  in: header\n  parameter: X-USER-ID\n  description: PlayHT user identifier paired with the API key.\n  sources:\n  - openapi/play-ht-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/play-ht/refs/heads/main/authentication/play-ht-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- AI
- Voice
- TTS
- Voice Cloning
- Audio
- Realtime
---
