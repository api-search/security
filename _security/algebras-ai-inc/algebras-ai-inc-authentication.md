---
api_key_in:
- header
api_specs:
- filename: algebras-ai-inc-authentication-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Authentication API
  slug: algebras-ai-inc-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-authentication-api-openapi.yml
- filename: algebras-ai-inc-common-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Common API
  slug: algebras-ai-inc-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-common-api-openapi.yml
- filename: algebras-ai-inc-glossaries-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Glossaries API
  slug: algebras-ai-inc-glossaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-glossaries-api-openapi.yml
- filename: algebras-ai-inc-languages-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Languages API
  slug: algebras-ai-inc-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-languages-api-openapi.yml
- filename: algebras-ai-inc-localization-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Localization API
  slug: algebras-ai-inc-localization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-localization-api-openapi.yml
- filename: algebras-ai-inc-realtime-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Realtime API
  slug: algebras-ai-inc-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-realtime-api-openapi.yml
- filename: algebras-ai-inc-storage-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Storage API
  slug: algebras-ai-inc-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-storage-api-openapi.yml
- filename: algebras-ai-inc-translation-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Translation API
  slug: algebras-ai-inc-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-translation-api-openapi.yml
- filename: algebras-ai-inc-video-api-openapi.yml
  format: yaml
  label: Algebras AI Inc. Video API
  slug: algebras-ai-inc-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-video-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Algebras Ai Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Algebras AI Inc. secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Algebras AI Inc.
provider_slug: algebras-ai-inc
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/algebras-ai-inc-openapi-original.json
  type: apiKey
slug: algebras-ai-inc-authentication
source_filename: algebras-ai-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/algebras-ai-inc-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/algebras-ai-inc-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/authentication/algebras-ai-inc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Translation
- Localization
- Internationalization
- Artificial Intelligence
- Machine Translation
- Voice
- Video
- Developer Tools
---
