---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: giveradar-com-charities-api-openapi.yml
  format: yaml
  label: GiveRadar Charities API
  slug: giveradar-com-charities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giveradar-com/openapi/giveradar-com-charities-api-openapi.yml
- filename: giveradar-com-platform-api-openapi.yml
  format: yaml
  label: GiveRadar Platform API
  slug: giveradar-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giveradar-com/openapi/giveradar-com-platform-api-openapi.yml
- filename: giveradar-com-reviews-api-openapi.yml
  format: yaml
  label: GiveRadar Reviews API
  slug: giveradar-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giveradar-com/openapi/giveradar-com-reviews-api-openapi.yml
- filename: giveradar-com-search-api-openapi.yml
  format: yaml
  label: GiveRadar Search API
  slug: giveradar-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giveradar-com/openapi/giveradar-com-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: GiveRadar Authentication
name_suffix: Authentication
oauth_flows: []
overview: GiveRadar secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GiveRadar
provider_slug: giveradar-com
scheme_count: 2
schemes:
- description: 'API key as Bearer token: `Authorization: Bearer gr_xxxxx`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/giveradar-com-openapi.yaml
  type: http
- description: 'API key as query parameter: `?api_key=gr_xxxxx`'
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/giveradar-com-openapi.yaml
  type: apiKey
slug: giveradar-com-authentication
source_filename: giveradar-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/giveradar-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key as Bearer token: `Authorization: Bearer gr_xxxxx`'\n  sources:\n  - openapi/giveradar-com-openapi.yaml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: 'API key as query parameter: `?api_key=gr_xxxxx`'\n  sources:\n  - openapi/giveradar-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/giveradar-com/authentication/giveradar-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Charity
- Data
- Non-Profit
- Global
---
