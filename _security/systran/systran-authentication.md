---
api_key_in:
- header
- query
api_specs:
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Translation API
  slug: systran-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN File Translation API
  slug: systran-file-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Supported Languages API
  slug: systran-supported-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Language Detection API
  slug: systran-language-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN NLP API
  slug: systran-nlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Dictionary API
  slug: systran-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Profiles API
  slug: systran-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Corpus API
  slug: systran-corpus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Systran Authentication
name_suffix: Authentication
oauth_flows: []
overview: SYSTRAN secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SYSTRAN
provider_slug: systran
scheme_count: 2
schemes:
- description: SYSTRAN API key passed as the `key` query parameter.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/systran-openapi.yml
  type: apiKey
- description: 'API key passed as an Authorization header, e.g. `Authorization: Key YOUR_API_KEY`.'
  in: header
  name: ApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/systran-openapi.yml
  type: apiKey
slug: systran-authentication
source_filename: systran-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/systran-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: SYSTRAN API key passed as the `key` query parameter.\n  sources:\n  - openapi/systran-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key passed as an Authorization header, e.g. `Authorization: Key YOUR_API_KEY`.'\n  sources:\n  - openapi/systran-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/authentication/systran-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Machine Translation
- Translation
- NLP
- Neural Machine Translation
- Localization
- Language Detection
---
