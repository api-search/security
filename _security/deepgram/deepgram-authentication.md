---
api_key_in:
- header
api_specs:
- filename: deepgram-voice-agent-asyncapi.yml
  format: yaml
  label: Deepgram Voice Agent API
  slug: voice-agent-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/asyncapi/deepgram-voice-agent-asyncapi.yml
- filename: deepgram-balances-api-openapi.yml
  format: yaml
  label: Deepgram Balances API
  slug: deepgram-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-balances-api-openapi.yml
- filename: deepgram-invitations-api-openapi.yml
  format: yaml
  label: Deepgram Invitations API
  slug: deepgram-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-invitations-api-openapi.yml
- filename: deepgram-keys-api-openapi.yml
  format: yaml
  label: Deepgram Keys API
  slug: deepgram-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-keys-api-openapi.yml
- filename: deepgram-members-api-openapi.yml
  format: yaml
  label: Deepgram Members API
  slug: deepgram-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-members-api-openapi.yml
- filename: deepgram-models-api-openapi.yml
  format: yaml
  label: Deepgram Models API
  slug: deepgram-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-models-api-openapi.yml
- filename: deepgram-pre-recorded-api-openapi.yml
  format: yaml
  label: Deepgram Pre-Recorded API
  slug: deepgram-pre-recorded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-pre-recorded-api-openapi.yml
- filename: deepgram-projects-api-openapi.yml
  format: yaml
  label: Deepgram Projects API
  slug: deepgram-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-projects-api-openapi.yml
- filename: deepgram-scopes-api-openapi.yml
  format: yaml
  label: Deepgram Scopes API
  slug: deepgram-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-scopes-api-openapi.yml
- filename: deepgram-text-intelligence-api-openapi.yml
  format: yaml
  label: Deepgram Text Intelligence API
  slug: deepgram-text-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-text-intelligence-api-openapi.yml
- filename: deepgram-text-to-speech-api-openapi.yml
  format: yaml
  label: Deepgram Text-To-Speech API
  slug: deepgram-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-text-to-speech-api-openapi.yml
- filename: deepgram-usage-api-openapi.yml
  format: yaml
  label: Deepgram Usage API
  slug: deepgram-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-usage-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deepgram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deepgram secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Deepgram
provider_slug: deepgram
scheme_count: 2
schemes:
- description: Deepgram API key passed as a bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deepgram-management-openapi.yml
  - openapi/deepgram-speech-to-text-openapi.yml
  - openapi/deepgram-text-to-speech-openapi.yml
  type: http
- description: Deepgram API key passed with Token prefix, e.g. Token YOUR_API_KEY.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/deepgram-speech-to-text-openapi.yml
  type: apiKey
slug: deepgram-authentication
source_filename: deepgram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepgram-management-openapi.yml, openapi/deepgram-speech-to-text-openapi.yml,\n  openapi/deepgram-text-to-speech-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Deepgram API key passed as a bearer token in the Authorization header.\n  sources:\n  - openapi/deepgram-management-openapi.yml\n  - openapi/deepgram-speech-to-text-openapi.yml\n  - openapi/deepgram-text-to-speech-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Deepgram API key passed with Token prefix, e.g. Token YOUR_API_KEY.\n  sources:\n  - openapi/deepgram-speech-to-text-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/authentication/deepgram-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Speech-to-Text
- Text-to-Speech
- Transcription
- Voice AI
---
