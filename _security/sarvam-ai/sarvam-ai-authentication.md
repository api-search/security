---
api_key_in:
- header
api_specs:
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Chat Completions (LLM) API
  slug: sarvam-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Speech-to-Text API
  slug: sarvam-ai-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Speech-to-Text Translate API
  slug: sarvam-ai-speech-to-text-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Text-to-Speech API
  slug: sarvam-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Translate API
  slug: sarvam-ai-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Transliterate API
  slug: sarvam-ai-transliterate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Language Identification API
  slug: sarvam-ai-language-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sarvam Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sarvam AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sarvam AI
provider_slug: sarvam-ai
scheme_count: 1
schemes:
- description: API subscription key created in the Sarvam AI dashboard.
  in: header
  name: ApiSubscriptionKey
  parameter: api-subscription-key
  sources:
  - openapi/sarvam-ai-openapi.yml
  type: apiKey
slug: sarvam-ai-authentication
source_filename: sarvam-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sarvam-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiSubscriptionKey\n  type: apiKey\n  in: header\n  parameter: api-subscription-key\n  description: API subscription key created in the Sarvam AI dashboard.\n  sources:\n  - openapi/sarvam-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/authentication/sarvam-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- LLM
- Speech to Text
- Text to Speech
- Translation
- Indian Languages
---
