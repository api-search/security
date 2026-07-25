---
api_key_in:
- header
api_specs:
- filename: modulate-velma-2-accent-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Accent Batch API
  slug: modulate-velma-2-accent-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-accent-batch-api-openapi.yml
- filename: modulate-velma-2-ai-music-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Ai Music Detection Batch API
  slug: modulate-velma-2-ai-music-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-ai-music-detection-batch-api-openapi.yml
- filename: modulate-velma-2-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Batch API
  slug: modulate-velma-2-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-batch-api-openapi.yml
- filename: modulate-velma-2-emotion-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Emotion Batch API
  slug: modulate-velma-2-emotion-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-emotion-batch-api-openapi.yml
- filename: modulate-velma-2-language-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Language Detection Batch API
  slug: modulate-velma-2-language-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-language-detection-batch-api-openapi.yml
- filename: modulate-velma-2-music-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Music Detection Batch API
  slug: modulate-velma-2-music-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-music-detection-batch-api-openapi.yml
- filename: modulate-velma-2-pii-phi-redaction-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Pii Phi Redaction Batch API
  slug: modulate-velma-2-pii-phi-redaction-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-pii-phi-redaction-batch-api-openapi.yml
- filename: modulate-velma-2-stt-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Stt Batch API
  slug: modulate-velma-2-stt-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-stt-batch-api-openapi.yml
- filename: modulate-velma-2-stt-batch-english-vfast-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Stt Batch English Vfast API
  slug: modulate-velma-2-stt-batch-english-vfast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-stt-batch-english-vfast-api-openapi.yml
- filename: modulate-velma-2-stt-batch-multilingual-vfast-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Stt Batch Multilingual Vfast API
  slug: modulate-velma-2-stt-batch-multilingual-vfast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-stt-batch-multilingual-vfast-api-openapi.yml
- filename: modulate-velma-2-synthetic-voice-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Synthetic Voice Detection Batch API
  slug: modulate-velma-2-synthetic-voice-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-synthetic-voice-detection-batch-api-openapi.yml
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
