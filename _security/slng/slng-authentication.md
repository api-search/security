---
api_key_in: []
api_specs:
- filename: slng-account-api-openapi.yml
  format: yaml
  label: SLNG Account API
  slug: slng-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-account-api-openapi.yml
- filename: slng-agents-api-openapi.yml
  format: yaml
  label: SLNG Agents API
  slug: slng-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-agents-api-openapi.yml
- filename: slng-calls-api-openapi.yml
  format: yaml
  label: SLNG Calls API
  slug: slng-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-calls-api-openapi.yml
- filename: slng-catalog-api-openapi.yml
  format: yaml
  label: SLNG Catalog API
  slug: slng-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-catalog-api-openapi.yml
- filename: slng-deepgram-aura-2-api-openapi.yml
  format: yaml
  label: SLNG Deepgram Aura 2 API
  slug: slng-deepgram-aura-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-deepgram-aura-2-api-openapi.yml
- filename: slng-deepgram-nova-3-api-openapi.yml
  format: yaml
  label: SLNG Deepgram Nova 3 API
  slug: slng-deepgram-nova-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-deepgram-nova-3-api-openapi.yml
- filename: slng-inworld-max-1-5-api-openapi.yml
  format: yaml
  label: SLNG Inworld Max 1.5 API
  slug: slng-inworld-max-1-5-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-inworld-max-1-5-api-openapi.yml
- filename: slng-orpheus-english-api-openapi.yml
  format: yaml
  label: SLNG Orpheus English API
  slug: slng-orpheus-english-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-orpheus-english-api-openapi.yml
- filename: slng-pronunciation-dictionaries-api-openapi.yml
  format: yaml
  label: SLNG Pronunciation dictionaries API
  slug: slng-pronunciation-dictionaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-pronunciation-dictionaries-api-openapi.yml
- filename: slng-rime-arcana-v2-api-openapi.yml
  format: yaml
  label: SLNG Rime Arcana v2 API
  slug: slng-rime-arcana-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-rime-arcana-v2-api-openapi.yml
- filename: slng-rime-arcana-v3-api-openapi.yml
  format: yaml
  label: SLNG Rime Arcana v3 API
  slug: slng-rime-arcana-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-rime-arcana-v3-api-openapi.yml
- filename: slng-rime-coda-api-openapi.yml
  format: yaml
  label: SLNG Rime Coda API
  slug: slng-rime-coda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-rime-coda-api-openapi.yml
- filename: slng-sessions-api-openapi.yml
  format: yaml
  label: SLNG Sessions API
  slug: slng-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-sessions-api-openapi.yml
- filename: slng-speechmatics-api-openapi.yml
  format: yaml
  label: SLNG Speechmatics API
  slug: slng-speechmatics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-speechmatics-api-openapi.yml
- filename: slng-whisper-large-v3-api-openapi.yml
  format: yaml
  label: SLNG Whisper Large v3 API
  slug: slng-whisper-large-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-whisper-large-v3-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Slng Authentication
name_suffix: Authentication
oauth_flows: []
overview: SLNG secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SLNG
provider_slug: slng
scheme_count: 1
schemes:
- bearerFormat: API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/slng-agents-openapi.yml
  - openapi/slng-batch-openapi.json
  - openapi/slng-management-slng-openapi.yml
  - openapi/slng-me-openapi.json
  - openapi/slng-stt-slng-openapi.yml
  - openapi/slng-tts-pronunciation-dictionaries-openapi.yml
  - openapi/slng-tts-slng-openapi.yml
  type: http
slug: slng-authentication
source_filename: slng-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.slng.ai/authentication.md\ndocs: https://docs.slng.ai/authentication.md\nsummary:\n  types:\n  - http\n  style: bearer-token\n  header: 'Authorization: Bearer <SLNG_API_KEY>'\n  key_management: Keys created/deleted at https://app.slng.ai/api-keys; secret shown once at creation, not retrievable later.\n  rotation: Keys cannot be rotated in place; create a new key and cut over, then delete the old one.\n  websocket_auth: Authorization header, or a `token` query parameter for browser clients that cannot set headers.\n  byok: Add an `X-Slng-Provider-Key` header alongside the SLNG key to run against your own upstream provider account (Bring Your Own Key).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/slng-agents-openapi.yml\n  - openapi/slng-batch-openapi.json\n  - openapi/slng-management-slng-openapi.yml\n  - openapi/slng-me-openapi.json\n  - openapi/slng-stt-slng-openapi.yml\n\
  \  - openapi/slng-tts-pronunciation-dictionaries-openapi.yml\n  - openapi/slng-tts-slng-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/authentication/slng-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Speech
- Voice
- Speech to Text
- Text to Speech
- Voice AI
- Voice Agents
- Transcription
- Speech Recognition
- Artificial Intelligence
- API Gateway
---
