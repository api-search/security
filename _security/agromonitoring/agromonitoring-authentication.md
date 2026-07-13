---
api_key_in:
- query
api_specs:
- filename: agromonitoring-openapi.yml
  format: yaml
  label: Agromonitoring
  slug: agromonitoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/openapi/agromonitoring-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agromonitoring Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agromonitoring secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agromonitoring
provider_slug: agromonitoring
scheme_count: 1
schemes:
- description: API key obtained by registering at agromonitoring.com. Append appid=YOUR_API_KEY to all API requests.
  in: query
  name: ApiKeyQuery
  parameter: appid
  sources:
  - openapi/agromonitoring-openapi.yml
  type: apiKey
slug: agromonitoring-authentication
source_filename: agromonitoring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agromonitoring-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: appid\n  description: API key obtained by registering at agromonitoring.com. Append appid=YOUR_API_KEY\n    to all API requests.\n  sources:\n  - openapi/agromonitoring-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/authentication/agromonitoring-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
---
