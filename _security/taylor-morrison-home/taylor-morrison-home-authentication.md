---
api_key_in:
- header
api_specs:
- filename: taylor-morrison-home-search-openapi.yml
  format: yaml
  label: Taylor Morrison Home Search API
  slug: taylor-morrison-home-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-search-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Taylor Morrison Home Authentication
name_suffix: Authentication
oauth_flows: []
overview: taylor-morrison-home secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: taylor-morrison-home
provider_slug: taylor-morrison-home
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/taylor-morrison-home-search-openapi.yml
  type: apiKey
slug: taylor-morrison-home-authentication
source_filename: taylor-morrison-home-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taylor-morrison-home-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/taylor-morrison-home-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/authentication/taylor-morrison-home-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Homebuilding
- Real Estate
- Fortune 1000
- New Homes
- Communities
- Mortgage
---
