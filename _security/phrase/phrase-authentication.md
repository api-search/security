---
api_key_in:
- header
api_specs:
- filename: phrase-strings-openapi-original.yaml
  format: yaml
  label: Phrase Strings API
  slug: phrase-strings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phrase/refs/heads/main/openapi/phrase-strings-openapi-original.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Phrase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phrase secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Phrase
provider_slug: phrase
scheme_count: 2
schemes:
- description: Enter your token in the format `token TOKEN`
  in: header
  name: Token
  parameter: Authorization
  sources:
  - openapi/phrase-strings-openapi-original.yaml
  type: apiKey
- name: Basic
  scheme: basic
  sources:
  - openapi/phrase-strings-openapi-original.yaml
  type: http
slug: phrase-authentication
source_filename: phrase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/phrase-strings-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Enter your token in the format `token TOKEN`\n  sources:\n  - openapi/phrase-strings-openapi-original.yaml\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/phrase-strings-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phrase/refs/heads/main/authentication/phrase-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Content Management
- Localization
- Translation
- Strings
- Internationalization
---
