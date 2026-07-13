---
api_key_in:
- header
api_specs:
- filename: lingo-dev-openapi.yml
  format: yaml
  label: Lingo.dev Engine API (Localize)
  slug: engine-api-localize
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/openapi/lingo-dev-openapi.yml
- filename: lingo-dev-openapi.yml
  format: yaml
  label: Lingo.dev SDK
  slug: sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/openapi/lingo-dev-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lingo Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lingo.dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lingo.dev
provider_slug: lingo-dev
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/lingo-dev-openapi.yml
  type: apiKey
slug: lingo-dev-authentication
source_filename: lingo-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lingo-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/lingo-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/authentication/lingo-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Localization
- Translation
- i18n
- Developer Tools
---
