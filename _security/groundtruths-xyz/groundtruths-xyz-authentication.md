---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GroundTruths Authentication
name_suffix: Authentication
oauth_flows: []
overview: GroundTruths secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GroundTruths
provider_slug: groundtruths-xyz
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/groundtruths-xyz-openapi.json
  type: apiKey
slug: groundtruths-xyz-authentication
source_filename: groundtruths-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/groundtruths-xyz-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/groundtruths-xyz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/groundtruths-xyz/authentication/groundtruths-xyz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Prediction-Market
- Betting
- Analytics
- Finance
---
