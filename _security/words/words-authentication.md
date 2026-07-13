---
api_key_in:
- header
api_specs:
- filename: words-openapi.yml
  format: yaml
  label: Words API
  slug: words-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Words Authentication
name_suffix: Authentication
oauth_flows: []
overview: Words API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Words API
provider_slug: words
scheme_count: 1
schemes:
- description: RapidAPI subscription key. The X-RapidAPI-Host header (wordsapiv1.p.rapidapi.com) is also required.
  in: header
  name: RapidApiKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/words-openapi.yml
  type: apiKey
slug: words-authentication
source_filename: words-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/words-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidApiKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: RapidAPI subscription key. The X-RapidAPI-Host header (wordsapiv1.p.rapidapi.com)\n    is also required.\n  sources:\n  - openapi/words-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/authentication/words-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Dictionaries
- Linguistics
- English
- Thesaurus
- Lexical Data
- Public APIs
---
