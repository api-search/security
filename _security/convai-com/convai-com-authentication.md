---
api_key_in:
- header
api_specs:
- filename: convai-com-characters-api-openapi.yml
  format: yaml
  label: Convai Characters API
  slug: convai-com-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-characters-api-openapi.yml
- filename: convai-com-chat-history-api-openapi.yml
  format: yaml
  label: Convai Chat History API
  slug: convai-com-chat-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-chat-history-api-openapi.yml
- filename: convai-com-custom-llm-api-openapi.yml
  format: yaml
  label: Convai Custom LLM API
  slug: convai-com-custom-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-custom-llm-api-openapi.yml
- filename: convai-com-evaluation-api-openapi.yml
  format: yaml
  label: Convai Evaluation API
  slug: convai-com-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-evaluation-api-openapi.yml
- filename: convai-com-interaction-api-openapi.yml
  format: yaml
  label: Convai Interaction API
  slug: convai-com-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-interaction-api-openapi.yml
- filename: convai-com-knowledge-bank-api-openapi.yml
  format: yaml
  label: Convai Knowledge Bank API
  slug: convai-com-knowledge-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-knowledge-bank-api-openapi.yml
- filename: convai-com-live-api-openapi.yml
  format: yaml
  label: Convai Live API
  slug: convai-com-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-live-api-openapi.yml
- filename: convai-com-narrative-api-openapi.yml
  format: yaml
  label: Convai Narrative API
  slug: convai-com-narrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-narrative-api-openapi.yml
- filename: convai-com-streaming-api-openapi.yml
  format: yaml
  label: Convai Streaming API
  slug: convai-com-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-streaming-api-openapi.yml
- filename: convai-com-tts-api-openapi.yml
  format: yaml
  label: Convai TTS API
  slug: convai-com-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-tts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Convai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convai secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Convai
provider_slug: convai-com
scheme_count: 2
schemes:
- in: header
  name: ConvaiApiKey
  parameter: CONVAI-API-KEY
  sources:
  - openapi/convai-character-api-openapi.yml
  - openapi/convai-chat-history-api-openapi.yml
  - openapi/convai-custom-llm-api-openapi.yml
  - openapi/convai-evaluation-api-openapi.yml
  - openapi/convai-interaction-api-openapi.yml
  - openapi/convai-knowledge-bank-api-openapi.yml
  - openapi/convai-narrative-design-api-openapi.yml
  - openapi/convai-streaming-transcription-api-openapi.yml
  - openapi/convai-tts-api-openapi.yml
  type: apiKey
- in: header
  name: LiveApiKey
  parameter: X-API-Key
  sources:
  - openapi/convai-live-api-openapi.yml
  type: apiKey
slug: convai-com-authentication
source_filename: convai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/convai-character-api-openapi.yml, openapi/convai-chat-history-api-openapi.yml,\n  openapi/convai-custom-llm-api-openapi.yml, openapi/convai-evaluation-api-openapi.yml, openapi/convai-interaction-api-openapi.yml,\n  openapi/convai-knowledge-bank-api-openapi.yml, openapi/convai-live-api-openapi.yml, openapi/convai-narrative-design-api-openapi.yml,\n  openapi/convai-streaming-transcription-api-openapi.yml, openapi/convai-tts-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ConvaiApiKey\n  type: apiKey\n  in: header\n  parameter: CONVAI-API-KEY\n  sources:\n  - openapi/convai-character-api-openapi.yml\n  - openapi/convai-chat-history-api-openapi.yml\n  - openapi/convai-custom-llm-api-openapi.yml\n  - openapi/convai-evaluation-api-openapi.yml\n  - openapi/convai-interaction-api-openapi.yml\n  - openapi/convai-knowledge-bank-api-openapi.yml\n  - openapi/convai-narrative-design-api-openapi.yml\n\
  \  - openapi/convai-streaming-transcription-api-openapi.yml\n  - openapi/convai-tts-api-openapi.yml\n- name: LiveApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/convai-live-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/authentication/convai-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- AI
- Conversational AI
- Characters
- NPCs
- Virtual Worlds
- Games
- Avatars
- Speech
- TTS
- WebRTC
---
