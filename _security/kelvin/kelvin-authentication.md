---
api_key_in: []
api_specs:
- filename: kelvin-documents-api-openapi.yml
  format: yaml
  label: Kelvin Documents API
  slug: kelvin-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/openapi/kelvin-documents-api-openapi.yml
- filename: kelvin-qualification-api-openapi.yml
  format: yaml
  label: Kelvin Qualification API
  slug: kelvin-qualification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/openapi/kelvin-qualification-api-openapi.yml
- filename: kelvin-simulateur-api-openapi.yml
  format: yaml
  label: Kelvin Simulateur API
  slug: kelvin-simulateur-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/openapi/kelvin-simulateur-api-openapi.yml
- filename: kelvin-simulations-api-openapi.yml
  format: yaml
  label: Kelvin Simulations API
  slug: kelvin-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/openapi/kelvin-simulations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kelvin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kelvin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kelvin
provider_slug: kelvin
scheme_count: 1
schemes:
- description: Le token commence par 'team-api-key-'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kelvin-api-openapi.yml
  - openapi/kelvin-api-v2-openapi.yml
  type: http
slug: kelvin-authentication
source_filename: kelvin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/kelvin-api-openapi.yml, openapi/kelvin-api-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Le token commence par 'team-api-key-'\n  sources:\n  - openapi/kelvin-api-openapi.yml\n  - openapi/kelvin-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/authentication/kelvin-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy
- Energy Efficiency
- Home Renovation
- Construction
- Artificial Intelligence
- Lead Generation
- Sales Enablement
- France
- Sustainability
---
