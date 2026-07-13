---
api_key_in:
- header
api_specs:
- filename: playht-asyncapi.yml
  format: yaml
  label: PlayAI Text-to-Speech API
  slug: tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/playht/refs/heads/main/asyncapi/playht-asyncapi.yml
- filename: playht-asyncapi.yml
  format: yaml
  label: PlayAI Voice Agents API
  slug: agents-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/playht/refs/heads/main/asyncapi/playht-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Playht Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlayHT secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PlayHT
provider_slug: playht
scheme_count: 2
schemes:
- description: Secret API key issued in the PlayAI console.
  in: header
  name: apiKey
  parameter: AUTHORIZATION
  sources:
  - openapi/playht-openapi.yml
  type: apiKey
- description: PlayAI user identifier paired with the API key.
  in: header
  name: userId
  parameter: X-USER-ID
  sources:
  - openapi/playht-openapi.yml
  type: apiKey
slug: playht-authentication
source_filename: playht-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/playht-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: AUTHORIZATION\n  description: Secret API key issued in the PlayAI console.\n  sources:\n  - openapi/playht-openapi.yml\n- name: userId\n  type: apiKey\n  in: header\n  parameter: X-USER-ID\n  description: PlayAI user identifier paired with the API key.\n  sources:\n  - openapi/playht-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playht/refs/heads/main/authentication/playht-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Voice
- TTS
- Text to Speech
- Voice Cloning
- Voice Agents
- Streaming
- PlayDialog
- Play 3.0
- PlayNote
- Multilingual
- Real-Time
---
