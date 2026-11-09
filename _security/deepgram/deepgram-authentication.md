---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: deepgram-voice-agent-asyncapi.yml
  format: yaml
  label: Deepgram Voice Agent API
  slug: voice-agent-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/deepgram/asyncapi/deepgram-voice-agent-asyncapi.yml
- filename: deepgram-balances-api-openapi.yml
  format: yaml
  label: Deepgram Balances API
  slug: deepgram-balances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-balances-api-openapi.yml
- filename: deepgram-keys-api-openapi.yml
  format: yaml
  label: Deepgram Keys API
  slug: deepgram-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-keys-api-openapi.yml
- filename: deepgram-members-api-openapi.yml
  format: yaml
  label: Deepgram Members API
  slug: deepgram-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-members-api-openapi.yml
- filename: deepgram-models-api-openapi.yml
  format: yaml
  label: Deepgram Models API
  slug: deepgram-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-models-api-openapi.yml
- filename: deepgram-projects-api-openapi.yml
  format: yaml
  label: Deepgram Projects API
  slug: deepgram-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-projects-api-openapi.yml
- filename: deepgram-scopes-api-openapi.yml
  format: yaml
  label: Deepgram Scopes API
  slug: deepgram-scopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-scopes-api-openapi.yml
- filename: deepgram-usage-api-openapi.yml
  format: yaml
  label: Deepgram Usage API
  slug: deepgram-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-usage-api-openapi.yml
- filename: deepgram-audio-api-openapi.yml
  format: yaml
  label: Deepgram Audio API
  slug: deepgram-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-audio-api-openapi.yml
- filename: deepgram-breakdown-api-openapi.yml
  format: yaml
  label: Deepgram Breakdown API
  slug: deepgram-breakdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-breakdown-api-openapi.yml
- filename: deepgram-configurations-api-openapi.yml
  format: yaml
  label: Deepgram Configurations API
  slug: deepgram-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-configurations-api-openapi.yml
- filename: deepgram-distributioncredentials-api-openapi.yml
  format: yaml
  label: Deepgram Distribution Credentials API
  slug: deepgram-distributioncredentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-distributioncredentials-api-openapi.yml
- filename: deepgram-fields-api-openapi.yml
  format: yaml
  label: Deepgram Fields API
  slug: deepgram-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-fields-api-openapi.yml
- filename: deepgram-invites-api-openapi.yml
  format: yaml
  label: Deepgram Invites API
  slug: deepgram-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-invites-api-openapi.yml
- filename: deepgram-media-api-openapi.yml
  format: yaml
  label: Deepgram Media API
  slug: deepgram-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-media-api-openapi.yml
- filename: deepgram-purchases-api-openapi.yml
  format: yaml
  label: Deepgram Purchases API
  slug: deepgram-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-purchases-api-openapi.yml
- filename: deepgram-requests-api-openapi.yml
  format: yaml
  label: Deepgram Requests API
  slug: deepgram-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-requests-api-openapi.yml
- filename: deepgram-text-api-openapi.yml
  format: yaml
  label: Deepgram Text API
  slug: deepgram-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-text-api-openapi.yml
- filename: deepgram-tokens-api-openapi.yml
  format: yaml
  label: Deepgram Tokens API
  slug: deepgram-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-tokens-api-openapi.yml
- filename: deepgram-variables-api-openapi.yml
  format: yaml
  label: Deepgram Variables API
  slug: deepgram-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-variables-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
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
source_yaml_url: https://artifacts.apis.io/deepgram/authentication/deepgram-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Speech-to-Text
- Text-to-Speech
- Transcription
- Voice AI
- Voice
- Real-Time
---
