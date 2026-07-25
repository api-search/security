---
api_key_in:
- header
- query
api_specs:
- filename: wordnik-account-api-openapi.yml
  format: yaml
  label: Wordnik Account API
  slug: wordnik-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/openapi/wordnik-account-api-openapi.yml
- filename: wordnik-word-api-openapi.yml
  format: yaml
  label: Wordnik Word API
  slug: wordnik-word-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/openapi/wordnik-word-api-openapi.yml
- filename: wordnik-word-list-api-openapi.yml
  format: yaml
  label: Wordnik Word List API
  slug: wordnik-word-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/openapi/wordnik-word-list-api-openapi.yml
- filename: wordnik-word-lists-api-openapi.yml
  format: yaml
  label: Wordnik Word Lists API
  slug: wordnik-word-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/openapi/wordnik-word-lists-api-openapi.yml
- filename: wordnik-words-api-openapi.yml
  format: yaml
  label: Wordnik Words API
  slug: wordnik-words-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/openapi/wordnik-words-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wordnik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wordnik secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wordnik
provider_slug: wordnik
scheme_count: 2
schemes:
- description: Wordnik issues per-account API keys; pass via the `api_key` query parameter on every request.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/wordnik-openapi.yml
  type: apiKey
- description: User auth token returned by `/account.json/authenticate/{username}`; required for user-scoped account and word-list operations.
  in: header
  name: auth_token
  parameter: auth_token
  sources:
  - openapi/wordnik-openapi.yml
  type: apiKey
slug: wordnik-authentication
source_filename: wordnik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wordnik-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Wordnik issues per-account API keys; pass via the `api_key` query parameter on\n    every request.\n  sources:\n  - openapi/wordnik-openapi.yml\n- name: auth_token\n  type: apiKey\n  in: header\n  parameter: auth_token\n  description: User auth token returned by `/account.json/authenticate/{username}`; required\n    for user-scoped account and word-list operations.\n  sources:\n  - openapi/wordnik-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/authentication/wordnik-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Dictionaries
- Dictionary
- Word Data
- English
- Lexicography
- Public APIs
---
