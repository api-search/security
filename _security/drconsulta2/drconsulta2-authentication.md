---
anonymous_access: false
api_key_in: []
api_specs:
- filename: drconsulta2-autentica-o-api-openapi.yml
  format: yaml
  label: Drconsulta2 Autenticação API
  slug: drconsulta2-autentica-o-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drconsulta2/openapi/drconsulta2-autentica-o-api-openapi.yml
- filename: drconsulta2-oracle-api-openapi.yml
  format: yaml
  label: Drconsulta2 Oracle API
  slug: drconsulta2-oracle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drconsulta2/openapi/drconsulta2-oracle-api-openapi.yml
- filename: drconsulta2-s2-api-openapi.yml
  format: yaml
  label: Drconsulta2 S2 API
  slug: drconsulta2-s2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drconsulta2/openapi/drconsulta2-s2-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Drconsulta2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drconsulta2 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drconsulta2
provider_slug: drconsulta2
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drconsulta2-openapi.json
  type: http
slug: drconsulta2-authentication
source_filename: drconsulta2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: derived\nsource: openapi/drconsulta2-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/drconsulta2-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/drconsulta2/authentication/drconsulta2-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
