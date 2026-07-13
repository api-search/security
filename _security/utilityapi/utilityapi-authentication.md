---
api_key_in: []
api_specs:
- filename: utilityapi-openapi.yml
  format: yaml
  label: UtilityAPI
  slug: utilityapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Utilityapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: UtilityAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UtilityAPI
provider_slug: utilityapi
scheme_count: 1
schemes:
- description: API token from the UtilityAPI dashboard
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/utilityapi-openapi.yml
  type: http
slug: utilityapi-authentication
source_filename: utilityapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/utilityapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token from the UtilityAPI dashboard\n  sources:\n  - openapi/utilityapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/authentication/utilityapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Utilities
- Green Button
- Billing Data
- Meter Data
- Clean Energy
---
