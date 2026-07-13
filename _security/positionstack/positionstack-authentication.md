---
api_key_in:
- query
api_specs:
- filename: positionstack-openapi.yml
  format: yaml
  label: positionstack Geocoding API
  slug: positionstack-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positionstack/refs/heads/main/openapi/positionstack-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Positionstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: positionstack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: positionstack
provider_slug: positionstack
scheme_count: 1
schemes:
- description: API access key obtained from your positionstack dashboard.
  in: query
  name: AccessKeyAuth
  parameter: access_key
  sources:
  - openapi/positionstack-openapi.yml
  type: apiKey
slug: positionstack-authentication
source_filename: positionstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/positionstack-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: AccessKeyAuth\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: API access key obtained from your positionstack dashboard.\n  sources:\n  - openapi/positionstack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/positionstack/refs/heads/main/authentication/positionstack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geocoding
- Reverse Geocoding
- Maps
- Location
- Address Validation
- apilayer
- Public APIs
---
