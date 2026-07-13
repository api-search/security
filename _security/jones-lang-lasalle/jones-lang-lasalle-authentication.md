---
api_key_in: []
api_specs:
- filename: jones-lang-lasalle-corrigo-rest-api-openapi.yml
  format: yaml
  label: JLL Corrigo Enterprise REST API
  slug: corrigo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/openapi/jones-lang-lasalle-corrigo-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jones Lang Lasalle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jones Lang LaSalle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jones Lang LaSalle
provider_slug: jones-lang-lasalle
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jones-lang-lasalle-corrigo-rest-api-openapi.yml
  type: http
slug: jones-lang-lasalle-authentication
source_filename: jones-lang-lasalle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jones-lang-lasalle-corrigo-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/jones-lang-lasalle-corrigo-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/authentication/jones-lang-lasalle-authentication.yml
summary_line: http · 1 scheme
tags:
- Commercial Real Estate
- Facility Management
- Asset Management
- Work Orders
- Fortune 500
---
