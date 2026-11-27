---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lenius-app-butikker-api-openapi.yml
  format: yaml
  label: lenius-app Butikker API
  slug: lenius-app-butikker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenius-app/openapi/lenius-app-butikker-api-openapi.yml
- filename: lenius-app-butikskategorier-api-openapi.yml
  format: yaml
  label: lenius-app Butikskategorier API
  slug: lenius-app-butikskategorier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenius-app/openapi/lenius-app-butikskategorier-api-openapi.yml
- filename: lenius-app-system-api-openapi.yml
  format: yaml
  label: lenius-app System API
  slug: lenius-app-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenius-app/openapi/lenius-app-system-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: lenius-app Authentication
name_suffix: Authentication
oauth_flows: []
overview: lenius-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: lenius-app
provider_slug: lenius-app
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lenius-app-openapi.json
  type: http
slug: lenius-app-authentication
source_filename: lenius-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lenius-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lenius-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lenius-app/authentication/lenius-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
