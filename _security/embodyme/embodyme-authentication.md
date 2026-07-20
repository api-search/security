---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Embodyme Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmbodyMe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EmbodyMe
provider_slug: embodyme
scheme_count: 1
schemes:
- description: All DigiSelf Realtime/Stream API requests are authenticated with a per-account API key sent in the x-api-key request header (documented as DIGISELF_API_KEY in the sample apps). API access is provisioned on the DigiSelf Business plan. Sample backends also carry an OPENAI_API_KEY for the OpenAI Realtime API leg, which is a separate third-party credential and not part of DigiSelf auth.
  in: header
  name: DigiselfApiKey
  parameter: x-api-key
  sources:
  - https://github.com/embodyme/digiself-realtime-api-sample
  type: apiKey
slug: embodyme-authentication
source_filename: embodyme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/embodyme/digiself-realtime-api-sample\ndocs: https://github.com/embodyme/digiself-realtime-api-sample/tree/main/quick-start-meeting-bot\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: DigiselfApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    All DigiSelf Realtime/Stream API requests are authenticated with a\n    per-account API key sent in the x-api-key request header (documented as\n    DIGISELF_API_KEY in the sample apps). API access is provisioned on the\n    DigiSelf Business plan. Sample backends also carry an OPENAI_API_KEY for the\n    OpenAI Realtime API leg, which is a separate third-party credential and not\n    part of DigiSelf auth.\n  sources:\n  - https://github.com/embodyme/digiself-realtime-api-sample\nnotes:\n- No OpenAPI/Swagger securityScheme is published; this profile is captured from\n  the official digiself-realtime-api-sample\
  \ repository documentation.\n- No OAuth2/OpenID Connect surface was found; auth is single API key only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embodyme/refs/heads/main/authentication/embodyme-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Avatars
- Digital Humans
- Neural Rendering
- Face Tracking
- Generative AI
- Video Generation
- Real-Time
- Streaming
- SDK
---
