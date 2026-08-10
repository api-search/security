---
api_key_in:
- header
api_specs:
- filename: skymind-model-upload-api-openapi.yml
  format: yaml
  label: Pathmind Model Upload API
  slug: skymind-model-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skymind/refs/heads/main/openapi/skymind-model-upload-api-openapi.yml
- filename: skymind-projects-api-openapi.yml
  format: yaml
  label: Pathmind Projects API
  slug: skymind-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skymind/refs/heads/main/openapi/skymind-projects-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Skymind Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pathmind secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pathmind
provider_slug: skymind
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: X-PM-API-TOKEN
  sources:
  - openapi/skymind-pathmind-openapi-original.yml
  type: apiKey
slug: skymind-authentication
source_filename: skymind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/skymind-pathmind-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-PM-API-TOKEN\n  sources:\n  - openapi/skymind-pathmind-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skymind/refs/heads/main/authentication/skymind-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Reinforcement Learning
- Simulation
- Optimization
- Supply Chain
- Manufacturing
- Defunct
---
