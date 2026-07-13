---
api_key_in:
- query
api_specs:
- filename: thesports-football-openapi.yml
  format: yaml
  label: TheSports Football API
  slug: football-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thesports/refs/heads/main/openapi/thesports-football-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Thesports Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheSports secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TheSports
provider_slug: thesports
scheme_count: 1
schemes:
- description: API key for authentication, obtained from TheSports developer portal.
  in: query
  name: ApiKeyAuth
  parameter: user_key
  sources:
  - openapi/thesports-football-openapi.yml
  type: apiKey
slug: thesports-authentication
source_filename: thesports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thesports-football-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: user_key\n  description: API key for authentication, obtained from TheSports developer portal.\n  sources:\n  - openapi/thesports-football-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thesports/refs/heads/main/authentication/thesports-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports
- Football
- Basketball
- Tennis
- Esports
- Data
- Real-Time
---
