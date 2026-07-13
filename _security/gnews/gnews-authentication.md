---
api_key_in:
- query
api_specs:
- filename: gnews-openapi.yml
  format: yaml
  label: GNews
  slug: gnews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnews/refs/heads/main/openapi/gnews-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gnews Authentication
name_suffix: Authentication
oauth_flows: []
overview: GNews secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GNews
provider_slug: gnews
scheme_count: 1
schemes:
- in: query
  name: apikeyQuery
  parameter: apikey
  sources:
  - openapi/gnews-openapi.yml
  type: apiKey
slug: gnews-authentication
source_filename: gnews-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gnews-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/gnews-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gnews/refs/heads/main/authentication/gnews-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Articles
- Headlines
- News
- Search
---
