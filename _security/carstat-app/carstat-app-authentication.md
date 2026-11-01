---
anonymous_access: false
api_key_in: []
api_specs:
- filename: carstat-app-recalls-api-openapi.yml
  format: yaml
  label: carstat-app Recalls API
  slug: carstat-app-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-recalls-api-openapi.yml
- filename: carstat-app-safety-ratings-api-openapi.yml
  format: yaml
  label: carstat-app Safety Ratings API
  slug: carstat-app-safety-ratings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-safety-ratings-api-openapi.yml
- filename: carstat-app-vehicle-specifications-api-openapi.yml
  format: yaml
  label: carstat-app Vehicle Specifications API
  slug: carstat-app-vehicle-specifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-vehicle-specifications-api-openapi.yml
- filename: carstat-app-vin-decoding-api-openapi.yml
  format: yaml
  label: carstat-app VIN Decoding API
  slug: carstat-app-vin-decoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-vin-decoding-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Carstat App Authentication
name_suffix: Authentication
oauth_flows: []
overview: carstat-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: carstat-app
provider_slug: carstat-app
scheme_count: 1
schemes:
- bearerFormat: API Token
  description: API token authentication. Get your token from the dashboard.
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/carstat-app-openapi.yaml
  type: http
slug: carstat-app-authentication
source_filename: carstat-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/carstat-app-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  description: API token authentication. Get your token from the dashboard.\n  sources:\n  - openapi/carstat-app-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/carstat-app/authentication/carstat-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automotive
- Data
- API
- Vehicle
---
