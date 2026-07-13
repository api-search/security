---
api_key_in:
- header
api_specs:
- filename: linguatools-collocations-openapi.yml
  format: yaml
  label: Linguatools Collocations API
  slug: collocations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linguatools/refs/heads/main/openapi/linguatools-collocations-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Linguatools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linguatools secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Linguatools
provider_slug: linguatools
scheme_count: 1
schemes:
- in: header
  name: RapidAPIKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/linguatools-collocations-openapi.yml
  type: apiKey
slug: linguatools-authentication
source_filename: linguatools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linguatools-collocations-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidAPIKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  sources:\n  - openapi/linguatools-collocations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linguatools/refs/heads/main/authentication/linguatools-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Collocations
- Dictionary
- English
- Language
- Linguistics
- NLP
---
