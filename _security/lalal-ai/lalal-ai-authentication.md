---
api_key_in:
- header
api_specs:
- filename: lalal-ai-batch-stem-separation-api-openapi.yml
  format: yaml
  label: LALAL.AI Batch Stem Separation API
  slug: lalal-ai-batch-stem-separation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-batch-stem-separation-api-openapi.yml
- filename: lalal-ai-common-api-openapi.yml
  format: yaml
  label: LALAL.AI Common API
  slug: lalal-ai-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-common-api-openapi.yml
- filename: lalal-ai-stem-separation-api-openapi.yml
  format: yaml
  label: LALAL.AI Stem Separation API
  slug: lalal-ai-stem-separation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-stem-separation-api-openapi.yml
- filename: lalal-ai-voice-change-api-openapi.yml
  format: yaml
  label: LALAL.AI Voice Change API
  slug: lalal-ai-voice-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-voice-change-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lalal Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: LALAL.AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LALAL.AI
provider_slug: lalal-ai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyHeaderAuth
  parameter: X-License-Key
  sources:
  - openapi/lalal-ai-api-openapi.yml
  type: apiKey
slug: lalal-ai-authentication
source_filename: lalal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lalal-ai-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeaderAuth\n  type: apiKey\n  in: header\n  parameter: X-License-Key\n  sources:\n  - openapi/lalal-ai-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/authentication/lalal-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Artificial Intelligence
- Audio
- Audio Processing
- Stem Separation
- Vocal Removal
- Voice Cleaning
- Voice Cloning
- Voice Changer
- Music
- Machine Learning
- DSP
---
