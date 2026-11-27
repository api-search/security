---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fish-audio-model-api-openapi.yml
  format: yaml
  label: Fish Audio Model API
  slug: fish-audio-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-model-api-openapi.yml
- filename: fish-audio-wallet-api-openapi.yml
  format: yaml
  label: Fish Audio Wallet API
  slug: fish-audio-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-wallet-api-openapi.yml
- filename: fish-audio-agent-sessions-api-openapi.yml
  format: yaml
  label: Fish Audio Agent Sessions API
  slug: fish-audio-agent-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agent-sessions-api-openapi.yml
- filename: fish-audio-agent-tests-api-openapi.yml
  format: yaml
  label: Fish Audio Agent Tests API
  slug: fish-audio-agent-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agent-tests-api-openapi.yml
- filename: fish-audio-agent-tools-api-openapi.yml
  format: yaml
  label: Fish Audio Agent Tools API
  slug: fish-audio-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agent-tools-api-openapi.yml
- filename: fish-audio-agents-api-openapi.yml
  format: yaml
  label: Fish Audio Agents API
  slug: fish-audio-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agents-api-openapi.yml
- filename: fish-audio-knowledge-sources-api-openapi.yml
  format: yaml
  label: Fish Audio Knowledge Sources API
  slug: fish-audio-knowledge-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-knowledge-sources-api-openapi.yml
- filename: fish-audio-openapi-v1-api-openapi.yml
  format: yaml
  label: Fish Audio OpenAPI v1 API
  slug: fish-audio-openapi-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-openapi-v1-api-openapi.yml
- filename: fish-audio-phone-calls-api-openapi.yml
  format: yaml
  label: Fish Audio Phone Calls API
  slug: fish-audio-phone-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-phone-calls-api-openapi.yml
- filename: fish-audio-phone-numbers-api-openapi.yml
  format: yaml
  label: Fish Audio Phone Numbers API
  slug: fish-audio-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-phone-numbers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fish Audio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fish Audio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fish Audio
provider_slug: fish-audio
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fish-audio-openapi.yml
  type: http
slug: fish-audio-authentication
source_filename: fish-audio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fish-audio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/fish-audio-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/fish-audio/authentication/fish-audio-authentication.yml
summary_line: http · 1 scheme
tags:
- Voice
- Text-to-Speech
- Speech-to-Text
- Voice Cloning
- Audio
- Generative AI
- Multilingual
- Streaming
- SDK
- Open Source
---
