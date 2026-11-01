---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gribstream-com-account-api-openapi.yml
  format: yaml
  label: gribstream-com Account API
  slug: gribstream-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-account-api-openapi.yml
- filename: gribstream-com-catalog-api-openapi.yml
  format: yaml
  label: gribstream-com Catalog API
  slug: gribstream-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-catalog-api-openapi.yml
- filename: gribstream-com-grid-coordinates-api-openapi.yml
  format: yaml
  label: gribstream-com Grid coordinates API
  slug: gribstream-com-grid-coordinates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-grid-coordinates-api-openapi.yml
- filename: gribstream-com-weather-data-api-openapi.yml
  format: yaml
  label: gribstream-com Weather data API
  slug: gribstream-com-weather-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-weather-data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gribstream Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: gribstream-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: gribstream-com
provider_slug: gribstream-com
scheme_count: 1
schemes:
- bearerFormat: API token
  description: 'Send your GribStream API token as:


    `Authorization: Bearer YOUR_TOKEN`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gribstream-com-openapi.yml
  type: http
slug: gribstream-com-authentication
source_filename: gribstream-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/gribstream-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API token\n  description: |-\n    Send your GribStream API token as:\n\n    `Authorization: Bearer YOUR_TOKEN`\n  sources:\n  - openapi/gribstream-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gribstream-com/authentication/gribstream-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Weather
- API
- Forecast
- Data
---
