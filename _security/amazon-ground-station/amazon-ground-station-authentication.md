---
api_key_in:
- header
api_specs:
- filename: amazon-ground-station-openapi.yaml
  format: yaml
  label: AWS Ground Station API
  slug: aws-ground-station-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Ground Station Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Ground Station secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-ground-station-openapi.yaml
  type: apiKey
slug: amazon-ground-station-authentication
source_filename: amazon-ground-station-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ground-station-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-ground-station-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/authentication/amazon-ground-station-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
---
