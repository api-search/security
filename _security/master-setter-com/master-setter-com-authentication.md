---
anonymous_access: false
api_key_in: []
api_specs:
- filename: master-setter-com-billing-api-openapi.yml
  format: yaml
  label: Master Setter Billing API
  slug: master-setter-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-billing-api-openapi.yml
- filename: master-setter-com-cards-api-openapi.yml
  format: yaml
  label: Master Setter Cards API
  slug: master-setter-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-cards-api-openapi.yml
- filename: master-setter-com-keys-api-openapi.yml
  format: yaml
  label: Master Setter Keys API
  slug: master-setter-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-keys-api-openapi.yml
- filename: master-setter-com-sets-api-openapi.yml
  format: yaml
  label: Master Setter Sets API
  slug: master-setter-com-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/master-setter-com/openapi/master-setter-com-sets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Master Setter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Master Setter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Master Setter
provider_slug: master-setter-com
scheme_count: 1
schemes:
- description: 'Authorization: Bearer mst_… (get one free from POST /v1/keys)'
  name: bearer
  scheme: bearer
  sources:
  - openapi/master-setter-com-openapi.json
  type: http
slug: master-setter-com-authentication
source_filename: master-setter-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/master-setter-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer mst_… (get one free from POST /v1/keys)'\n  sources:\n  - openapi/master-setter-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/master-setter-com/authentication/master-setter-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Pokemon
- TCG
- Collection
- Data
---
