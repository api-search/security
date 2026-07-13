---
api_key_in:
- query
api_specs:
- filename: weglot-openapi.yml
  format: yaml
  label: Weglot Translate API
  slug: weglot-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/openapi/weglot-openapi.yml
- filename: weglot-openapi.yml
  format: yaml
  label: Weglot Languages API
  slug: weglot-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/openapi/weglot-openapi.yml
- filename: weglot-openapi.yml
  format: yaml
  label: Weglot Status API
  slug: weglot-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/openapi/weglot-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Weglot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weglot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weglot
provider_slug: weglot
scheme_count: 1
schemes:
- description: Weglot project API key passed as the api_key query parameter.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/weglot-openapi.yml
  type: apiKey
slug: weglot-authentication
source_filename: weglot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weglot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Weglot project API key passed as the api_key query parameter.\n  sources:\n  - openapi/weglot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/authentication/weglot-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Translation
- Localization
- Internationalization
- Machine Translation
- Multilingual
---
