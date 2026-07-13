---
api_key_in:
- header
api_specs:
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Translation API
  slug: unbabel-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Machine Translation API
  slug: unbabel-machine-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Language Pairs API
  slug: unbabel-language-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Tone and Topic API
  slug: unbabel-tone-topic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Word Count API
  slug: unbabel-word-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Account API
  slug: unbabel-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Notifications API
  slug: unbabel-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Unbabel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unbabel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unbabel
provider_slug: unbabel
scheme_count: 1
schemes:
- description: 'Token authentication of the form `Authorization: ApiKey <username>:<api_key>`.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/unbabel-openapi.yml
  type: apiKey
slug: unbabel-authentication
source_filename: unbabel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unbabel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token authentication of the form `Authorization: ApiKey <username>:<api_key>`.'\n  sources:\n  - openapi/unbabel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/authentication/unbabel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Translation
- Localization
- Language Operations
- LangOps
- Machine Translation
- Human in the Loop
- AI
---
