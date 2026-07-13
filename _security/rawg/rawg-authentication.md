---
api_key_in:
- query
api_specs:
- filename: rawg-openapi.yml
  format: yaml
  label: RAWG Video Games Database API
  slug: rawg
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rawg/refs/heads/main/openapi/rawg-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rawg Authentication
name_suffix: Authentication
oauth_flows: []
overview: RAWG secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RAWG
provider_slug: rawg
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/rawg-openapi.yml
  type: apiKey
slug: rawg-authentication
source_filename: rawg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rawg-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/rawg-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rawg/refs/heads/main/authentication/rawg-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Database
- Entertainment
- Game Discovery
- Games
- Gaming
- Metadata
- Video Games
---
