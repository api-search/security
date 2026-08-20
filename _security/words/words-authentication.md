---
api_key_in:
- header
api_specs:
- filename: words-categories-api-openapi.yml
  format: yaml
  label: Words API Categories API
  slug: words-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-categories-api-openapi.yml
- filename: words-definitions-api-openapi.yml
  format: yaml
  label: Words API Definitions API
  slug: words-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-definitions-api-openapi.yml
- filename: words-examples-api-openapi.yml
  format: yaml
  label: Words API Examples API
  slug: words-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-examples-api-openapi.yml
- filename: words-frequency-api-openapi.yml
  format: yaml
  label: Words API Frequency API
  slug: words-frequency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-frequency-api-openapi.yml
- filename: words-hierarchy-api-openapi.yml
  format: yaml
  label: Words API Hierarchy API
  slug: words-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-hierarchy-api-openapi.yml
- filename: words-phonetics-api-openapi.yml
  format: yaml
  label: Words API Phonetics API
  slug: words-phonetics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-phonetics-api-openapi.yml
- filename: words-search-api-openapi.yml
  format: yaml
  label: Words API Search API
  slug: words-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-search-api-openapi.yml
- filename: words-thesaurus-api-openapi.yml
  format: yaml
  label: Words API Thesaurus API
  slug: words-thesaurus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-thesaurus-api-openapi.yml
- filename: words-word-api-openapi.yml
  format: yaml
  label: Words API Word API
  slug: words-word-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-word-api-openapi.yml
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
- thesaurus
- Lexical Data
- Public APIs
---
