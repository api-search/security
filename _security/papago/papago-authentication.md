---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Papago NMT Translation API
  slug: papago-nmt-translation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papago/refs/heads/main/openapi/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Papago Authentication
name_suffix: Authentication
oauth_flows: []
overview: Papago secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Papago
provider_slug: papago
scheme_count: 2
schemes:
- description: Client ID issued when registering an application on the Naver Developer Center.
  in: header
  name: clientId
  parameter: X-Naver-Client-Id
  sources:
  - openapi/openapi.yaml
  type: apiKey
- description: Client secret issued when registering an application on the Naver Developer Center.
  in: header
  name: clientSecret
  parameter: X-Naver-Client-Secret
  sources:
  - openapi/openapi.yaml
  type: apiKey
slug: papago-authentication
source_filename: papago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: X-Naver-Client-Id\n  description: Client ID issued when registering an application on the Naver Developer Center.\n  sources:\n  - openapi/openapi.yaml\n- name: clientSecret\n  type: apiKey\n  in: header\n  parameter: X-Naver-Client-Secret\n  description: Client secret issued when registering an application on the Naver Developer Center.\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/papago/refs/heads/main/authentication/papago-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Translation
- Natural Language Processing
- Machine Translation
- Neural Machine Translation
- Korean
- Asian Languages
- Localization
- Language Detection
---
