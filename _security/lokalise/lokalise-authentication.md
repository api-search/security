---
api_key_in:
- header
api_specs:
- filename: lokalise-openapi.yml
  format: yaml
  label: Lokalise API v2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lokalise/refs/heads/main/openapi/lokalise-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lokalise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lokalise secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lokalise
provider_slug: lokalise
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Token
  sources:
  - openapi/lokalise-openapi.yml
  type: apiKey
slug: lokalise-authentication
source_filename: lokalise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lokalise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Token\n  sources:\n  - openapi/lokalise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lokalise/refs/heads/main/authentication/lokalise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Localization
- Translation
- TMS
- AI Machine Translation
- REST
- Developer Tools
---
