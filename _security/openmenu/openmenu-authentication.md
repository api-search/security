---
api_key_in:
- query
api_specs:
- filename: openmenu-openapi.yml
  format: yaml
  label: OpenMenu API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmenu/refs/heads/main/openapi/openmenu-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openmenu Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMenu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenMenu
provider_slug: openmenu
scheme_count: 1
schemes:
- description: API key issued from your OpenMenu account, passed as the `key` query parameter on every request. There is no Bearer token or custom header.
  in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/openmenu-openapi.yml
  type: apiKey
slug: openmenu-authentication
source_filename: openmenu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openmenu-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key issued from your OpenMenu account, passed as the `key` query parameter\n    on every request. There is no Bearer token or custom header.\n  sources:\n  - openapi/openmenu-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmenu/refs/heads/main/authentication/openmenu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Menus
- Menu Data
- Search
- Nutrition
- Structured Data
---
