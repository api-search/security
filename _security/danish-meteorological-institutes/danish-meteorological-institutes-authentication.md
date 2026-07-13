---
api_key_in:
- query
api_specs:
- filename: dmi-open-data-api-openapi.yml
  format: yaml
  label: DMI Open Data API
  slug: dmi-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/openapi/dmi-open-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Danish Meteorological Institutes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Danish Meteorological Institutes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Danish Meteorological Institutes
provider_slug: danish-meteorological-institutes
scheme_count: 1
schemes:
- description: Per-service API key issued by the DMI Open Data portal.
  in: query
  name: apiKey
  parameter: api-key
  sources:
  - openapi/dmi-open-data-api-openapi.yml
  type: apiKey
slug: danish-meteorological-institutes-authentication
source_filename: danish-meteorological-institutes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dmi-open-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api-key\n  description: Per-service API key issued by the DMI Open Data portal.\n  sources:\n  - openapi/dmi-open-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/authentication/danish-meteorological-institutes-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Climate
- Environment
- Lightning
- Meteorological
- Ocean
- Open Data
- Weather
---
