---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: Yandex Translate API
  slug: yandex-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yandex Translate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yandex Translate API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yandex Translate API
provider_slug: yandex-translate
scheme_count: 2
schemes:
- description: 'IAM token obtained from Yandex Identity and Access Management (IAM). Pass as ''Authorization: Bearer <IAM_TOKEN>''.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
- description: 'API key for service accounts. Pass as ''Authorization: Api-Key <API_KEY>''.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: yandex-translate-authentication
source_filename: yandex-translate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'IAM token obtained from Yandex Identity and Access Management (IAM). Pass as\n    ''Authorization: Bearer <IAM_TOKEN>''.'\n  sources:\n  - openapi/openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key for service accounts. Pass as ''Authorization: Api-Key <API_KEY>''.'\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/authentication/yandex-translate-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Machine Translation
- Natural Language Processing
- Language Detection
- Translation Dictionary
- Multilingual
- Yandex Cloud
- Localization
- Internationalization
---
