---
api_key_in:
- header
api_specs:
- filename: velma-2-batch-openapi-original.yml
  format: yaml
  label: Velma-2 Voice Intelligence API
  slug: velma-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/velma-2-batch-openapi-original.yml
- filename: stt-batch-openapi-original.yml
  format: yaml
  label: Speech-to-Text Transcription API
  slug: stt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/stt-batch-openapi-original.yml
- filename: synthetic-voice-detection-batch-openapi-original.yml
  format: yaml
  label: Deepfake (Synthetic Voice) Detection API
  slug: deepfake-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/synthetic-voice-detection-batch-openapi-original.yml
- filename: pii-phi-redaction-batch-openapi-original.yml
  format: yaml
  label: PII/PHI Redaction API
  slug: pii-phi-redaction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/pii-phi-redaction-batch-openapi-original.yml
- filename: emotion-batch-openapi-original.yml
  format: yaml
  label: Emotion Detection API
  slug: emotion-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/emotion-batch-openapi-original.yml
- filename: accent-batch-openapi-original.yml
  format: yaml
  label: Accent Detection API
  slug: accent-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/accent-batch-openapi-original.yml
- filename: language-detection-batch-openapi-original.yml
  format: yaml
  label: Language Detection API
  slug: language-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/language-detection-batch-openapi-original.yml
- filename: music-detection-batch-openapi-original.yml
  format: yaml
  label: Music & Speech Detection API
  slug: music-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/music-detection-batch-openapi-original.yml
- filename: ai-music-detection-batch-openapi-original.yml
  format: yaml
  label: AI Music Detection API
  slug: ai-music-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/ai-music-detection-batch-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Modulate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modulate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Modulate
provider_slug: modulate
scheme_count: 1
schemes:
- description: API key used for authentication and usage tracking.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/accent-batch-openapi-original.yml
  - openapi/ai-music-detection-batch-openapi-original.yml
  - openapi/emotion-batch-openapi-original.yml
  - openapi/language-detection-batch-openapi-original.yml
  - openapi/music-detection-batch-openapi-original.yml
  - openapi/pii-phi-redaction-batch-openapi-original.yml
  - openapi/stt-batch-english-vfast-openapi-original.yml
  - openapi/stt-batch-multilingual-vfast-openapi-original.yml
  - openapi/stt-batch-openapi-original.yml
  - openapi/synthetic-voice-detection-batch-openapi-original.yml
  - openapi/velma-2-batch-openapi-original.yml
  type: apiKey
slug: modulate-authentication
source_filename: modulate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/accent-batch-openapi-original.yml, openapi/ai-music-detection-batch-openapi-original.yml,\n  openapi/emotion-batch-openapi-original.yml, openapi/language-detection-batch-openapi-original.yml,\n  openapi/music-detection-batch-openapi-original.yml, openapi/pii-phi-redaction-batch-openapi-original.yml,\n  openapi/stt-batch-english-vfast-openapi-original.yml, openapi/stt-batch-multilingual-vfast-openapi-original.yml,\n  openapi/stt-batch-openapi-original.yml, openapi/synthetic-voice-detection-batch-openapi-original.yml,\n  openapi/velma-2-batch-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key used for authentication and usage tracking.\n  sources:\n  - openapi/accent-batch-openapi-original.yml\n  - openapi/ai-music-detection-batch-openapi-original.yml\n  - openapi/emotion-batch-openapi-original.yml\n\
  \  - openapi/language-detection-batch-openapi-original.yml\n  - openapi/music-detection-batch-openapi-original.yml\n  - openapi/pii-phi-redaction-batch-openapi-original.yml\n  - openapi/stt-batch-english-vfast-openapi-original.yml\n  - openapi/stt-batch-multilingual-vfast-openapi-original.yml\n  - openapi/stt-batch-openapi-original.yml\n  - openapi/synthetic-voice-detection-batch-openapi-original.yml\n  - openapi/velma-2-batch-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/authentication/modulate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Voice AI
- Speech to Text
- Transcription
- Deepfake Detection
- Content Moderation
- Trust and Safety
- Audio
- Machine Learning
- PII Redaction
- Voice Intelligence
---
