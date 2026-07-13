---
api_key_in:
- header
api_specs:
- filename: deepl-translation-api-openapi.yml
  format: yaml
  label: DeepL Translation API
  slug: deepl-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/openapi/deepl-translation-api-openapi.yml
- filename: deepl-voice-api-openapi.yml
  format: yaml
  label: DeepL Voice API
  slug: deepl-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/openapi/deepl-voice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Deepl Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeepL
provider_slug: deepl
scheme_count: 1
schemes:
- description: DeepL-Auth-Key <key>
  in: header
  name: authKey
  parameter: Authorization
  sources:
  - openapi/deepl-translation-api-openapi.yml
  - openapi/deepl-voice-api-openapi.yml
  type: apiKey
slug: deepl-authentication
source_filename: deepl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepl-translation-api-openapi.yml, openapi/deepl-voice-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: DeepL-Auth-Key <key>\n  sources:\n  - openapi/deepl-translation-api-openapi.yml\n  - openapi/deepl-voice-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/authentication/deepl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Deep Learning
- Glossaries
- Localization
- Machine Learning
- Machine Translation
- Translation
---
