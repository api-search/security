---
api_key_in:
- header
api_specs:
- filename: docs
  format: yaml
  label: SimpleLocalize Translation API
  slug: translation-api
  spec_type: OpenAPI
  url: https://api.simplelocalize.io/openapi/docs
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Simplelocalize Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleLocalize secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SimpleLocalize
provider_slug: simplelocalize
scheme_count: 2
schemes:
- description: Project API key from Settings > Credentials > API Key
  in: header
  name: ApiKeyAuth
  parameter: X-SimpleLocalize-Token
  sources:
  - openapi/simplelocalize-openapi.yml
  type: apiKey
- description: Personal Token for Projects API. Generated in account settings.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/simplelocalize-openapi.yml
  type: http
slug: simplelocalize-authentication
source_filename: simplelocalize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simplelocalize-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-SimpleLocalize-Token\n  description: Project API key from Settings > Credentials > API Key\n  sources:\n  - openapi/simplelocalize-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal Token for Projects API. Generated in account settings.\n  sources:\n  - openapi/simplelocalize-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/authentication/simplelocalize-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Localization
- Translation
- Internationalization
---
