---
api_key_in: []
api_specs:
- filename: funeralone-openapi.yml
  format: yaml
  label: funeralOne Cases API
  slug: funeralone-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/funeralone/refs/heads/main/openapi/funeralone-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Funeralone Authentication
name_suffix: Authentication
oauth_flows: []
overview: funeralOne secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: funeralOne
provider_slug: funeralone
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use the funeralOne-issued API key as the username and a blank/dummy password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/funeralone-openapi.yml
  type: http
slug: funeralone-authentication
source_filename: funeralone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/funeralone-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use the funeralOne-issued API key as the username\n    and a blank/dummy password.\n  sources:\n  - openapi/funeralone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funeralone/refs/heads/main/authentication/funeralone-authentication.yml
summary_line: http · 1 scheme
tags:
- Funeral Homes
- Deathcare
- Obituaries
- Tribute Videos
- Memorial Websites
- Life Tributes
- Case Management
- Partner API
---
