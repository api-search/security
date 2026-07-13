---
api_key_in:
- header
api_specs:
- filename: pexels-openapi.yml
  format: yaml
  label: Pexels API
  slug: pexels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexels/refs/heads/main/openapi/pexels-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pexels Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pexels secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pexels
provider_slug: pexels
scheme_count: 1
schemes:
- description: 'Pexels uses an API-key in the `Authorization` request header.

    Send your key as `Authorization: YOUR_API_KEY` on every request.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/pexels-openapi.yml
  type: apiKey
slug: pexels-authentication
source_filename: pexels-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pexels-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Pexels uses an API-key in the `Authorization` request header.\n    Send your key as `Authorization: YOUR_API_KEY` on every request.\n  sources:\n  - openapi/pexels-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexels/refs/heads/main/authentication/pexels-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Photos
- Stock Media
- Videos
---
