---
api_key_in:
- header
api_specs:
- filename: tavus-conversations-api-openapi.yml
  format: yaml
  label: Tavus Conversations API
  slug: tavus-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-conversations-api-openapi.yml
- filename: tavus-documents-api-openapi.yml
  format: yaml
  label: Tavus Documents API
  slug: tavus-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-documents-api-openapi.yml
- filename: tavus-guardrails-api-openapi.yml
  format: yaml
  label: Tavus Guardrails API
  slug: tavus-guardrails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-guardrails-api-openapi.yml
- filename: tavus-lipsync-api-openapi.yml
  format: yaml
  label: Tavus Lipsync API
  slug: tavus-lipsync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-lipsync-api-openapi.yml
- filename: tavus-objectives-api-openapi.yml
  format: yaml
  label: Tavus Objectives API
  slug: tavus-objectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-objectives-api-openapi.yml
- filename: tavus-personas-api-openapi.yml
  format: yaml
  label: Tavus Personas API
  slug: tavus-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-personas-api-openapi.yml
- filename: tavus-pronunciation-dictionaries-api-openapi.yml
  format: yaml
  label: Tavus Pronunciation Dictionaries API
  slug: tavus-pronunciation-dictionaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-pronunciation-dictionaries-api-openapi.yml
- filename: tavus-replacements-api-openapi.yml
  format: yaml
  label: Tavus Replacements API
  slug: tavus-replacements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-replacements-api-openapi.yml
- filename: tavus-replicas-api-openapi.yml
  format: yaml
  label: Tavus Replicas API
  slug: tavus-replicas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-replicas-api-openapi.yml
- filename: tavus-transcriptions-api-openapi.yml
  format: yaml
  label: Tavus Transcriptions API
  slug: tavus-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-transcriptions-api-openapi.yml
- filename: tavus-videos-api-openapi.yml
  format: yaml
  label: Tavus Videos API
  slug: tavus-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-videos-api-openapi.yml
- filename: tavus-voices-api-openapi.yml
  format: yaml
  label: Tavus Voices API
  slug: tavus-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-voices-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tavus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tavus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tavus
provider_slug: tavus
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/tavus-openapi.yml
  type: apiKey
slug: tavus-authentication
source_filename: tavus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tavus-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/tavus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/authentication/tavus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Generative AI
- Video
- Conversational AI
- Avatars
- Replicas
- Personalization
- Real Time
- CVI
- Webhooks
---
