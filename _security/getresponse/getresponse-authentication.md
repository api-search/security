---
api_key_in:
- header
api_specs:
- filename: getresponse-openapi.yml
  format: yaml
  label: GetResponse API v3
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Getresponse Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetResponse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GetResponse
provider_slug: getresponse
scheme_count: 1
schemes:
- description: 'Personal API key sent as "api-key YOUR_API_KEY". Keys expire after 90

    days of inactivity.'
  in: header
  name: apiKey
  parameter: X-Auth-Token
  sources:
  - openapi/getresponse-openapi.yml
  type: apiKey
slug: getresponse-authentication
source_filename: getresponse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/getresponse-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: |-\n    Personal API key sent as \"api-key YOUR_API_KEY\". Keys expire after 90\n    days of inactivity.\n  sources:\n  - openapi/getresponse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/authentication/getresponse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Landing Pages
- Webinars
- Conversion Funnels
- CRM
---
