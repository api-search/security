---
api_key_in:
- header
api_specs:
- filename: regal-cinema-openapi.yml
  format: yaml
  label: Regal Cinema API
  slug: regal-cinema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/openapi/regal-cinema-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Regal Entertainment Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: regal-entertainment-group secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: regal-entertainment-group
provider_slug: regal-entertainment-group
scheme_count: 1
schemes:
- description: Azure API Management subscription key from developer.regmovies.com
  in: header
  name: ApiKeyAuth
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/regal-cinema-openapi.yml
  type: apiKey
slug: regal-entertainment-group-authentication
source_filename: regal-entertainment-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regal-cinema-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Azure API Management subscription key from developer.regmovies.com\n  sources:\n  - openapi/regal-cinema-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/authentication/regal-entertainment-group-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cinema
- Entertainment
- Movies
- Ticketing
- Loyalty
- Theatre
- Fortune 500
---
