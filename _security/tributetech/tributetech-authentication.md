---
api_key_in: []
api_specs:
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Authentication API
  slug: tributetech-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Serving Locations API
  slug: tributetech-serving-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Obituaries API
  slug: tributetech-obituaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tributetech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tribute Technology secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tribute Technology
provider_slug: tributetech
scheme_count: 1
schemes:
- description: 'HTML bearer token obtained from POST /token/. Include as Authorization: Bearer {TOKEN}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tributetech-openapi.yml
  type: http
slug: tributetech-authentication
source_filename: tributetech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tributetech-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'HTML bearer token obtained from POST /token/. Include as Authorization: Bearer\n    {TOKEN}.'\n  sources:\n  - openapi/tributetech-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/authentication/tributetech-authentication.yml
summary_line: http · 1 scheme
tags:
- Funeral Technology
- Obituaries
- Memorials
- Funeral Homes
- E-commerce
- Death Care
- Case Management
---
