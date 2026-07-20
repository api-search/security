---
api_key_in:
- header
api_specs:
- filename: definedcrowd-openapi-original.json
  format: json
  label: Defined.ai Public API
  slug: definedai-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/definedcrowd/refs/heads/main/openapi/definedcrowd-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Definedcrowd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Defined.ai (DefinedCrowd) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Defined.ai (DefinedCrowd)
provider_slug: definedcrowd
scheme_count: 1
schemes:
- description: Please enter into field the word 'Bearer' following by space and JWT
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/definedcrowd-openapi-original.json
  type: apiKey
slug: definedcrowd-authentication
source_filename: definedcrowd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/definedcrowd-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Please enter into field the word 'Bearer' following by space and JWT\n  sources:\n  - openapi/definedcrowd-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/definedcrowd/refs/heads/main/authentication/definedcrowd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Training Data
- Data Marketplace
- Machine Learning
- Data Annotation
- Speech Data
- Natural Language Processing
- Crowdsourcing
- Artificial Intelligence
---
