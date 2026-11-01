---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tessie-driver-management-api-openapi.yml
  format: yaml
  label: Tessie Driver Management API
  slug: tessie-driver-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-driver-management-api-openapi.yml
- filename: tessie-telemetry-configuration-api-openapi.yml
  format: yaml
  label: Tessie Telemetry Configuration API
  slug: tessie-telemetry-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-telemetry-configuration-api-openapi.yml
- filename: tessie-vehicle-commands-api-openapi.yml
  format: yaml
  label: Tessie Vehicle Commands API
  slug: tessie-vehicle-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-vehicle-commands-api-openapi.yml
- filename: tessie-vehicle-data-api-openapi.yml
  format: yaml
  label: Tessie Vehicle Data API
  slug: tessie-vehicle-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-vehicle-data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tessie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tessie secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tessie
provider_slug: tessie
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tessie-openapi.yaml
  type: http
slug: tessie-authentication
source_filename: tessie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/tessie-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tessie-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/tessie/authentication/tessie-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Tesla
- Fleet Management
- Automotive
- APIs
---
