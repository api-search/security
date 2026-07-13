---
api_key_in:
- query
api_specs:
- filename: europeana-openapi.yml
  format: yaml
  label: Europeana Search and Record API
  slug: europeana-search-and-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/europeana/refs/heads/main/openapi/europeana-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Europeana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Europeana secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Europeana
provider_slug: europeana
scheme_count: 1
schemes:
- description: Europeana API key. Register at https://pro.europeana.eu/pages/get-api.
  in: query
  name: apiKeyAuth
  parameter: wskey
  sources:
  - openapi/europeana-openapi.yml
  type: apiKey
slug: europeana-authentication
source_filename: europeana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/europeana-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: wskey\n  description: Europeana API key. Register at https://pro.europeana.eu/pages/get-api.\n  sources:\n  - openapi/europeana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/europeana/refs/heads/main/authentication/europeana-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Archives
- Cultural Heritage
- Europe
- Libraries
- Museums
- Search
---
