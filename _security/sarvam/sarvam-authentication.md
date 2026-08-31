---
api_key_in:
- header
api_specs:
- filename: sarvam-chat-api-openapi.yml
  format: yaml
  label: Sarvam chat API
  slug: sarvam-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-chat-api-openapi.yml
- filename: sarvam-documentintelligence-api-openapi.yml
  format: yaml
  label: Sarvam documentIntelligence API
  slug: sarvam-documentintelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-documentintelligence-api-openapi.yml
- filename: sarvam-pronunciationdictionary-api-openapi.yml
  format: yaml
  label: Sarvam pronunciationDictionary API
  slug: sarvam-pronunciationdictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-pronunciationdictionary-api-openapi.yml
- filename: sarvam-speechtotext-api-openapi.yml
  format: yaml
  label: Sarvam speechToText API
  slug: sarvam-speechtotext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-speechtotext-api-openapi.yml
- filename: sarvam-speechtotextjob-api-openapi.yml
  format: yaml
  label: Sarvam speechToTextJob API
  slug: sarvam-speechtotextjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-speechtotextjob-api-openapi.yml
- filename: sarvam-speechtotexttranslatejob-api-openapi.yml
  format: yaml
  label: Sarvam speechToTextTranslateJob API
  slug: sarvam-speechtotexttranslatejob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-speechtotexttranslatejob-api-openapi.yml
- filename: sarvam-text-api-openapi.yml
  format: yaml
  label: Sarvam text API
  slug: sarvam-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-text-api-openapi.yml
- filename: sarvam-texttospeech-api-openapi.yml
  format: yaml
  label: Sarvam textToSpeech API
  slug: sarvam-texttospeech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-texttospeech-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sarvam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sarvam secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sarvam
provider_slug: sarvam
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: api-subscription-key
  sources:
  - openapi/sarvam-openapi-original.json
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/sarvam-openapi-original.json
  type: http
slug: sarvam-authentication
source_filename: sarvam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sarvam-openapi-original.json\ndocs: https://docs.sarvam.ai/api-reference/authentication\nnotes: >-\n  Primary auth is an API key sent in the `api-subscription-key` header;\n  `Authorization: Bearer <key>` is also accepted. Keys are generated manually\n  in the Sarvam dashboard. Authentication failures return HTTP 403 (not 401)\n  with error.code `invalid_api_key_error`. The SDK also reads SARVAM_API_KEY.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api-subscription-key\n  sources:\n  - openapi/sarvam-openapi-original.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sarvam-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/authentication/sarvam-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Machine-Learning
- Speech To Text
- Text-to-Speech
- Translation
- Large Language Models
- Document Intelligence
- Indian Languages
- Voice
---
